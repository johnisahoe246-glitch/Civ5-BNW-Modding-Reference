{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetProjectProductionNeeded<b>(</b>{{Type5|ProjectType}} project<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|project:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|3142}}<syntaxhighlight lang="lua">cost = Players[Game.GetActivePlayer()]:GetProjectProductionNeeded( projectID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0305}}<syntaxhighlight lang="lua">local iCost = pActivePlayer:GetProjectProductionNeeded(iProjectID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetProjectProductionNeeded]]
[[Category:Civ5 City Production API|GetProjectProductionNeeded]]
[[Category:Civ5 Buildings API|GetProjectProductionNeeded]]