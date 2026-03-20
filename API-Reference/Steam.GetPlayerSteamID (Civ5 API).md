{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Steam}}.<br/>
This is a static method, invoke it with a dot.
}}


Returns the Steam ID information for a specific Player


=Usage=
<code>table('''unknown''' => '''unknown''') Steam.GetPlayerSteamID<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Returned Value'''
:Returns a table with the following fields:
::PlayerName
:Their current steam display name
::IsOnline
:Are they online?
::ID
:a 64-bit integer represented as a string pertaining to their ID.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''The player's Game ID, typically between 0 and #Players;''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
-- Print all player's SteamIDs
for i,v in ipairs(Players) do
if(v:IsHuman() then
local steamID = Steam.GetPlayerSteamID(i);
print(string.format("[%i] %s - %s", i, steamID.PlayerName, steamID.ID);
else
print(string.format("[%i] Computer", i);
end
end</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPlayerSteamID]]
[[Category:Civ5 Players API|GetPlayerSteamID]]