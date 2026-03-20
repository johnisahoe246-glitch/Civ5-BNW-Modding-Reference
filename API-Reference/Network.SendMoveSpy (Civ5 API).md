{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendMoveSpy<b>(</b>{{Type5|PlayerID}} arg0, '''unknown''' SelectedAgentID, {{Type5|PlayerID}} arg2, '''int''' arg3<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|SelectedAgentID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg3:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0328}}<syntaxhighlight lang="lua">Network.SendMoveSpy(Game.GetActivePlayer(), g_SelectedAgentID, -1, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1050}}<syntaxhighlight lang="lua">Network.SendMoveSpy(Game.GetActivePlayer(), selectedAgentIndex, v.PlayerID, v.CityID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendMoveSpy]]
[[Category:Civ5 Movement API|SendMoveSpy]]
[[Category:Civ5 Espionnage API|SendMoveSpy]]