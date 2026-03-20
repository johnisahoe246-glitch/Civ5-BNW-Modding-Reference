''This page is a part of the [[Lua and UI Reference (Civ5)|Lua and UI Reference]].''


=Types terminology=
{| cellpadding="8"
|-
|valign="top"|
* <code>'''unknown'''</code>
|This parameter's type could not be identified.
|-
|valign="top"|
* <code>'''string'''</code>
|A Lua string.
|-
|valign="top"|
* <code>'''int'''</code>
|Any integer.
|-
|valign="top"|
* <code>'''float'''</code>
|Any number, integer or floating-point.
|-
|valign="top"|
* <code>'''table'''</code>
|An unidentified table. Look at the code samples to figure it out by yourself.
|-
|valign="top"|
* <code>'''table(key => value)'''</code>
|A table whose keys and values have the specified types.
:Example: <code>table({{Type5|PlayerID}} => {{Type5|Player}}) players</code>
::It can be enumerated with: <code>for playerID, player in ipairs(players) do</code>
::The following will return a {{Type5|Player}}: <code>players[0]</code>
|-
|valign="top"|
* <code>'''iterator(type1, type2, type3)'''</code>
|To be used in a <code>for... in...</code> loop.
:Example: <code>iterator({{Type5|Unit}}) Units()</code> 
::It can be enumerated with: <code>for pUnit in Units() do</code>.
|-
|valign="top"|
* <code>'''variant'''</code>
|This parameter can be assigned with different types.
:Example: <code>DB.{{Func5|DB|Query}}('''variant''' arg)</code> 
::This function can accept a string or a table.
|-
|valign="top"|
* <code>'''...'''</code>
|A variable number of arguments. A good example is Locale.{{Func5|Locale|ConvertTextKey}}.
|}


=Object-oriented concepts in Lua=
The concepts below originate from object-oriented languages. But since Lua is weakly typed, it offers richer possibilities than those languages. As a result those concepts may sometimes lack relevance and may need to be adapted or broaden. However they're still adequate since most of the API reflects the types defined in C++ by Firaxis.


'''Instance versus static types'''
* Instance types can be instanced, such as {{Type5|Player}}. 
* Static types exist as a single global variable, such as {{Type5|Game}}. 
* Some types can be both, such as {{Type5|InstanceManager}}: a global variable exists with this name and calling its {{Func5|InstanceManager|new}} method creates a new instance of {{Type5|InstanceManager}}.


'''Functions versus methods'''
* We call method any function stored as a type member.
* This is purely aesthetic: a function and a method are both called and used in the same way. We could store a method in a local variable and use it as a function.


'''Instance methods'''
* They are methods that require the caller to be passed as the first argument.
* The colon (''':''') operator implicitly passes the caller as the first argument. Those two expressions are equivalent: <code>caller.somefunc(caller, arg)</code> and <code>caller:somefunc(arg)</code>
* When declaring methods, the caller is referenced as the '''self''' keyword. It can be explicitly defined or not, see [[Lua introduction for confirmed developers]].


'''Events'''
* Events in the civ5 API can be (un-)subscribed this way: <code>Events.SomeEvent.Add(Handler)</code> and <code>Events.SomeEvent.Remove(Handler)</code>
* They can be invoked like regular methods: <code>Events.SomeEvent(arg1, arg2)</code>
* Events typically do not expect any return type. But the ones in {{Type5|GameEvents}} usually expect an integer or a boolean, see their documentations.


=Reliability of the documentation=
'''All listed functions exist.'''
:But some of them may be malfunctioning. Ghost functions have been removed by checking the binaries strings tables.

'''Some functions may not be listed.'''
:Only the methods that can be enumerated by a Lua code, the ones mentioned on the 2k wiki, and the ones used by the Lua source code from Firaxis are listed. A few additional functions found in the binaries have been added but this scan is quite superficial.

'''Some functions could have hidden arguments/return types.'''
:There could be additional arguments not listed because they were never used or documented by Firaxis. 

'''Some functions arguments could be actually optional.'''
:Reciprocally, some of the arguments listed could be optional: Firaxis always used them but it does not mean they always need to be used.

'''Arguments' default values are not reliable.'''
:They are mostly here to notify you that an argument is optional. While '''nil''' is always an acceptable value to provide in such a case, a nil for a boolean will probably be interpreted as '''false''' (but it could be '''true''') and an integer as '''0''' (but it could be anything else).

'''The arguments' types and returned types are not always reliable.'''
:While a lot of efforts were done to ensure the typing is reliable, this problem cannot be solved unambiguously. The current compromise between truthfulness and completeness is quite good but it could still be improved and, anyway, it cannot be perfect without human corrections.

'''Most of those types are only here for documentation purpose'''
:The structures and identifiers are never mentioned anywhere in the API, they have been introduced for documentation purposes only. Lua and the API just treat them as tables (for structures) and integers (for identifiers). That being said, the structures obviously have C++ counterparts behind them. There could be additional structures that are not listed.


=Pages generation process=
The initial versions of those pages were automatically generated by a bot written in C# by [[User:DonQuich|DonQuiche]]. 

Here are the first steps of this bot:
* We manually define the existing type names and their natures (identifier, structure, etc)
* The [http://wiki.2kgames.com/civ5/index.php/Lua_Game_Objects 2kgames wiki] is scanned. It is sparse, the types are rarely mentioned and the informations are sometimes incorrect or obsolete.
* Manual fixes are applied to core functions that will trigger type inference cascades later during the Lua source code analysis.
* Two lua dumps (with and without G&K) are scanned to collect members. They have been generated by a home-brewed mod that outputs the members on all types, enumerations and their metatables.
* The binaries are scanned to detect additional functions for a few types. The process is rudimentary and does not collect many informations.
* The database files are scanned, this will be used to infere types from calls to GameInfos and such during the Lua source code analysis.


Then we parse the Lua and UI source files from the base game, G&K and most DLC. This step produces an inference graph and assembles the code samples. This is the main information source for the bot and the most important step.
* The inference graph is a bastardized version of a minimalist AST (abstract syntax tree), specialized for type equations resolution. It describes relations such as: ''argument 0 in SomeType.SomeFunc is assigned by the third return type of OtherType.OtherFunc, and also by...''.
* The inference graph is solved in order to infer all the arguments and return types. During this process we also update the arguments name, we detect unknown functions and arguments, new events, structures' fields, etc.
* The whole process implements its custom version of the VFS to manage includes. It manages to test all the possible combinations of different file versions to simulate the presence of absence of the expansions and DLC.


Finally, the whole API is known and the type system complete. 
* The binaries (dll and exe) are scanned a second time to search for all the strings they contain. If a function's name does not appear in those tables, it means it no longer exists. This is the primary source to detect methods that have been removed (from the base game and/or G&K) and, while simple, it is very reliable.
* We then import manually written texts to be included in some of the generated pages.
* Finally we consolidate everything and we categorize the methods according to the keywords found in their names.
* All pages are generated using T4 templates and we upload the new wiki thanks to the [http://dotnetwikibot.sourceforge.net/ DotNetWikiBot] library.


[[Category:Civ5 API]]