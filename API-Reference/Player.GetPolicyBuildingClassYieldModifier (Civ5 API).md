{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetPolicyBuildingClassYieldModifier<b>(</b>{{Type5|BuildingClassType}} buildingClass, {{Type5|YieldType}} arg1<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|buildingClass:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0167}}<syntaxhighlight lang="lua">iGold = iGold + pActivePlayer:GetPolicyBuildingClassYieldModifier(buildingClassID, YieldTypes.YIELD_GOLD);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0185}}<syntaxhighlight lang="lua">iScience = iScience + pActivePlayer:GetPolicyBuildingClassYieldModifier(buildingClassID, YieldTypes.YIELD_SCIENCE);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0200}}<syntaxhighlight lang="lua">iProduction = iProduction + pActivePlayer:GetPolicyBuildingClassYieldModifier(buildingClassID, YieldTypes.YIELD_PRODUCTION);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPolicyBuildingClassYieldModifier]]
[[Category:Civ5 Yields API|GetPolicyBuildingClassYieldModifier]]
[[Category:Civ5 Buildings API|GetPolicyBuildingClassYieldModifier]]
[[Category:Civ5 Policies API|GetPolicyBuildingClassYieldModifier]]