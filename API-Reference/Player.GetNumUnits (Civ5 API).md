{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNumUnits<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0283}}<syntaxhighlight lang="lua">local iTotalUnits = pPlayer:GetNumUnits();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">Controls.SupplyUseValue:SetText(        pPlayer:GetNumUnits() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">Controls.SupplyRemainingValue:SetText( pPlayer:GetNumUnitsSupplied() - pPlayer:GetNumUnits() );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumUnits]]
[[Category:Civ5 Units API|GetNumUnits]]