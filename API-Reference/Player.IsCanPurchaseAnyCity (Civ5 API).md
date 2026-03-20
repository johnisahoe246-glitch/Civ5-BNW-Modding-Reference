{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:IsCanPurchaseAnyCity<b>(</b>'''bool''' arg0, '''bool''' arg1, {{Type5|UnitType}} arg2, {{Type5|BuildingType}} arg3, {{Type5|YieldType}} arg4<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg3:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg4:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0450}}<syntaxhighlight lang="lua">if(faithCost > 0 and player:IsCanPurchaseAnyCity(false, true, unit.ID, -1, YieldTypes.YIELD_FAITH)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0458}}<syntaxhighlight lang="lua">if(faithCost > 0 and player:IsCanPurchaseAnyCity(false, true, -1, building.ID, YieldTypes.YIELD_FAITH)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsCanPurchaseAnyCity]]
[[Category:Civ5 Cities API|IsCanPurchaseAnyCity]]
[[Category:Civ5 City Production API|IsCanPurchaseAnyCity]]