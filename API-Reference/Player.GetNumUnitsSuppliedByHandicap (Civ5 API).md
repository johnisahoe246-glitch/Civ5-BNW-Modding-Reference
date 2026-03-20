{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNumUnitsSuppliedByHandicap<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0094}}<syntaxhighlight lang="lua">Controls.HandicapSupplyValue:SetText(   pPlayer:GetNumUnitsSuppliedByHandicap() );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumUnitsSuppliedByHandicap]]
[[Category:Civ5 Units API|GetNumUnitsSuppliedByHandicap]]
[[Category:Civ5 Game Settings API|GetNumUnitsSuppliedByHandicap]]