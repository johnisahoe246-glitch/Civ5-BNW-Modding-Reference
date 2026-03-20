{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetBuildingGoldMaintenance<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0318}}<syntaxhighlight lang="lua">Controls.BuildingExpenseValue:SetText( Locale.ToNumber( pPlayer:GetBuildingGoldMaintenance(), "#.##" ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0450}}<syntaxhighlight lang="lua">local iBuildingMaintenance = pPlayer:GetBuildingGoldMaintenance();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBuildingGoldMaintenance]]
[[Category:Civ5 Buildings API|GetBuildingGoldMaintenance]]
[[Category:Civ5 Gold API|GetBuildingGoldMaintenance]]