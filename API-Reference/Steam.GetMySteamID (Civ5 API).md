{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Steam}}.<br/>
This is a static method, invoke it with a dot.
}}


Returns information about the current user's Steam ID


=Usage=
<code>table('''unknown''' => '''unknown''') Steam.GetMySteamID<b>(</b><b>)</b></code>


'''Returned Value'''
:Returns a table with the following fields:
::PlayerName
:Your current steam display name
::IsOnline
:Are you online?
::ID
:a 64-bit integer represented as a string pertaining to your ID.


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local mySteamID = Steam.GetMySteamID();
print(mySteamID.PlayerName .. " - " .. mySteamID.ID);</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMySteamID]]