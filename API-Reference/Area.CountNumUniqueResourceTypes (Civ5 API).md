{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Area}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Area:CountNumUniqueResourceTypes<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0143}}<syntaxhighlight lang="lua">local numUniqueResourcesOnArea = area:CountNumUniqueResourceTypes() + 1; -- number of unique resources starting on the area, plus this one</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CountNumUniqueResourceTypes]]
[[Category:Civ5 Resources API|CountNumUniqueResourceTypes]]