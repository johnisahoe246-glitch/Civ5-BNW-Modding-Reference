{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' City:IsCanPurchase<b>(</b>{{Type5|UnitType}} unitType, '''int''' buildingType, '''int''' projectType, '''int''' projectID, '''int''' projectID = nil, {{Type5|YieldType}} yield = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|unitType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|buildingType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|projectType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|projectID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|projectID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|yield:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0288}}<syntaxhighlight lang="lua">if city:IsCanPurchase(true, unitID, -1, -1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0292}}<syntaxhighlight lang="lua">if (not city:IsCanPurchase(false, unitID, -1, -1)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0345}}<syntaxhighlight lang="lua">if city:IsCanPurchase(true, -1, -1, projectID) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0387}}<syntaxhighlight lang="lua">if city:IsCanPurchase(true, -1, buildingID, -1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0395}}<syntaxhighlight lang="lua">if (not city:IsCanPurchase(false, -1, buildingID, -1)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">if (city:IsCanPurchase(true, true, iData, -1, -1, eYield)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0116}}<syntaxhighlight lang="lua">if (city:IsCanPurchase(true, true, -1, iData, -1, eYield)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0120}}<syntaxhighlight lang="lua">if (city:IsCanPurchase(true, true, -1, -1, iData, eYield)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0344}}<syntaxhighlight lang="lua">if city:IsCanPurchase(false, false, unitID, -1, -1, YieldTypes.YIELD_GOLD) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0348}}<syntaxhighlight lang="lua">if (not city:IsCanPurchase(true, true, unitID, -1, -1, YieldTypes.YIELD_GOLD)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0356}}<syntaxhighlight lang="lua">if city:IsCanPurchase(false, false, unitID, -1, -1, YieldTypes.YIELD_FAITH) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0360}}<syntaxhighlight lang="lua">if (not city:IsCanPurchase(true, true, unitID, -1, -1, YieldTypes.YIELD_FAITH)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0414}}<syntaxhighlight lang="lua">if city:IsCanPurchase(false, false, -1, -1, projectID, YieldTypes.YIELD_GOLD) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0456}}<syntaxhighlight lang="lua">if city:IsCanPurchase(false, false, -1, buildingID, -1, YieldTypes.YIELD_GOLD) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0464}}<syntaxhighlight lang="lua">if (not city:IsCanPurchase(true, true, -1, buildingID, -1, YieldTypes.YIELD_GOLD)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0475}}<syntaxhighlight lang="lua">elseif city:IsCanPurchase(false, false, -1, buildingID, -1, YieldTypes.YIELD_FAITH) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0483}}<syntaxhighlight lang="lua">if (not city:IsCanPurchase(true, true, -1, buildingID, -1, YieldTypes.YIELD_FAITH)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsCanPurchase]]
[[Category:Civ5 City Production API|IsCanPurchase]]