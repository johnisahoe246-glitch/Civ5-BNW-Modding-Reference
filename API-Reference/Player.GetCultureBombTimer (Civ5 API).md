{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetCultureBombTimer<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1185}}<syntaxhighlight lang="lua">elseif (action.Type == "MISSION_CULTURE_BOMB" and pActivePlayer:GetCultureBombTimer() > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1193}}<syntaxhighlight lang="lua">strDisabledString = strDisabledString .. Locale.ConvertTextKey("TXT_KEY_MISSION_CULTURE_BOMB_DISABLED_COOLDOWN", pActivePlayer:GetCultureBombTimer());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCultureBombTimer]]
[[Category:Civ5 Culture API|GetCultureBombTimer]]