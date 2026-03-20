{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetUnitProductionMaintenanceMod<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0107}}<syntaxhighlight lang="lua">Controls.SupplyDeficitPenaltyValue:SetText( pPlayer:GetUnitProductionMaintenanceMod() .. "%" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">local iUnitSupplyMod = pPlayer:GetUnitProductionMaintenanceMod();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetUnitProductionMaintenanceMod]]
[[Category:Civ5 City Production API|GetUnitProductionMaintenanceMod]]
[[Category:Civ5 Units API|GetUnitProductionMaintenanceMod]]