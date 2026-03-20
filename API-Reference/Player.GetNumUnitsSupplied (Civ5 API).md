{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNumUnitsSupplied<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0097}}<syntaxhighlight lang="lua">Controls.SupplyCapValue:SetText(        pPlayer:GetNumUnitsSupplied() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">Controls.SupplyRemainingValue:SetText( pPlayer:GetNumUnitsSupplied() - pPlayer:GetNumUnits() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0211}}<syntaxhighlight lang="lua">local iUnitsSupplied = pPlayer:GetNumUnitsSupplied();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumUnitsSupplied]]
[[Category:Civ5 Units API|GetNumUnitsSupplied]]