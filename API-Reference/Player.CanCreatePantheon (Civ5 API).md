{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:CanCreatePantheon<b>(</b>'''bool''' arg0<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">elseif(player:CanCreatePantheon(true)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">elseif(player:CanCreatePantheon(false)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0950}}<syntaxhighlight lang="lua">if (pPlayer:CanCreatePantheon(false)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanCreatePantheon]]
[[Category:Civ5 City Production API|CanCreatePantheon]]
[[Category:Civ5 Religion API|CanCreatePantheon]]