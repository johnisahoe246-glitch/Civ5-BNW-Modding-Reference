{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.GetBuildingYieldChange<b>(</b>{{Type5|BuildingType}} building, {{Type5|YieldType}} arg1<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|building:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2779}}<syntaxhighlight lang="lua">return Game.GetBuildingYieldChange(buildingID, YieldTypes[yieldType]);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0159}}<syntaxhighlight lang="lua">local iFood = Game.GetBuildingYieldChange(iBuildingID, YieldTypes.YIELD_FOOD);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0175}}<syntaxhighlight lang="lua">iGold = Game.GetBuildingYieldChange(iBuildingID, YieldTypes.YIELD_GOLD);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0192}}<syntaxhighlight lang="lua">local iScienceChange = Game.GetBuildingYieldChange(iBuildingID, YieldTypes.YIELD_SCIENCE);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0207}}<syntaxhighlight lang="lua">local iProd = Game.GetBuildingYieldChange(iBuildingID, YieldTypes.YIELD_PRODUCTION);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">local iCulture = Game.GetBuildingYieldChange(iBuildingID, YieldTypes.YIELD_CULTURE);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0163}}<syntaxhighlight lang="lua">local iFaith = Game.GetBuildingYieldChange(iBuildingID, YieldTypes.YIELD_FAITH);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0217}}<syntaxhighlight lang="lua">local iScienceChange = Game.GetBuildingYieldChange(iBuildingID, YieldTypes.YIELD_SCIENCE) + pActivePlayer:GetPolicyBuildingClassYieldChange(buildingClassID, YieldTypes.YIELD_SCIENCE);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBuildingYieldChange]]
[[Category:Civ5 Yields API|GetBuildingYieldChange]]
[[Category:Civ5 Buildings API|GetBuildingYieldChange]]