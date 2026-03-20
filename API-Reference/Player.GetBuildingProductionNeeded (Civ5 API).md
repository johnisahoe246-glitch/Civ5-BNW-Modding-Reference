{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetBuildingProductionNeeded<b>(</b>'''int''' building<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|building:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2733}}<syntaxhighlight lang="lua">cost = Players[Game.GetActivePlayer()]:GetBuildingProductionNeeded( buildingID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0114}}<syntaxhighlight lang="lua">local iCost = pActivePlayer:GetBuildingProductionNeeded(iBuildingID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBuildingProductionNeeded]]
[[Category:Civ5 City Production API|GetBuildingProductionNeeded]]
[[Category:Civ5 Buildings API|GetBuildingProductionNeeded]]