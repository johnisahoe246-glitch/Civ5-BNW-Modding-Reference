{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetUnitFaithPurchaseCost<b>(</b>{{Type5|UnitType}} unit, '''bool''' arg1<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|unit:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ProductionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0365}}<syntaxhighlight lang="lua">local cost = city:GetUnitFaithPurchaseCost( unitID, true );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0423}}<syntaxhighlight lang="lua">local faithCost = capital:GetUnitFaithPurchaseCost(GameInfo.Units[v2].ID, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0449}}<syntaxhighlight lang="lua">local faithCost = capital:GetUnitFaithPurchaseCost(unit.ID, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetUnitFaithPurchaseCost]]
[[Category:Civ5 City Production API|GetUnitFaithPurchaseCost]]
[[Category:Civ5 Religion API|GetUnitFaithPurchaseCost]]
[[Category:Civ5 Units API|GetUnitFaithPurchaseCost]]