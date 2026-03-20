{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''string''' Locale.ToNumber<b>(</b>'''int''' netGPT, '''string''' arg1<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|netGPT:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 116 are listed.''

{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0135}}<syntaxhighlight lang="lua">instance.Best:SetText( Locale.ToNumber(best[1], "#,###,###,###") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0138}}<syntaxhighlight lang="lua">instance.Average:SetText( Locale.ToNumber( GetAverage( m_PopulationTable, iPlayer ), "#,###,###,###" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0143}}<syntaxhighlight lang="lua">instance.Worst:LocalizeAndSetText( Locale.ToNumber(worst[1], "#,###,###,###" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0146}}<syntaxhighlight lang="lua">instance.Rank:SetText( Locale.ToNumber(GetRank( m_PopulationTable, iPlayer ), "#") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0165}}<syntaxhighlight lang="lua">instance.Value:SetText( Locale.ToNumber(m_FoodTable[ iPlayer ], "#,###,###,###" ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0173}}<syntaxhighlight lang="lua">instance.Average:SetText( Locale.ToNumber( GetAverage( m_FoodTable, iPlayer ), "#,###,###,###" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0181}}<syntaxhighlight lang="lua">instance.Rank:SetText( Locale.ToNumber(GetRank( m_FoodTable, iPlayer ), "#") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0200}}<syntaxhighlight lang="lua">instance.Value:SetText( Locale.ToNumber(m_ProductionTable[ iPlayer ], "#,###,###,###" ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0208}}<syntaxhighlight lang="lua">instance.Average:SetText( Locale.ToNumber( GetAverage( m_ProductionTable, iPlayer ), "#,###,###,###" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0236}}<syntaxhighlight lang="lua">instance.Value:SetText( Locale.ToNumber(m_GoldTable[ iPlayer ], "#,###,###,###" ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0244}}<syntaxhighlight lang="lua">instance.Average:SetText( Locale.ToNumber( GetAverage( m_GoldTable, iPlayer ), "#,###,###,###" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0252}}<syntaxhighlight lang="lua">instance.Rank:SetText( Locale.ToNumber(GetRank( m_GoldTable, iPlayer ), "#") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0271}}<syntaxhighlight lang="lua">instance.Value:SetText( Locale.ToNumber(m_LandTable[ iPlayer ], "#,###,###,###" ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0279}}<syntaxhighlight lang="lua">instance.Average:SetText( Locale.ToNumber( GetAverage( m_LandTable, iPlayer ), "#,###,###,###" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0287}}<syntaxhighlight lang="lua">instance.Rank:SetText( Locale.ToNumber(GetRank( m_LandTable, iPlayer ), "#") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0306}}<syntaxhighlight lang="lua">instance.Value:SetText( Locale.ToNumber(m_ArmyTable[ iPlayer ], "#,###,###,###" ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0314}}<syntaxhighlight lang="lua">instance.Average:SetText( Locale.ToNumber( GetAverage( m_ArmyTable, iPlayer ), "#,###,###,###" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0319}}<syntaxhighlight lang="lua">instance.Worst:LocalizeAndSetText( Locale.ToNumber(worst[1], "#,###,###,###") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0368}}<syntaxhighlight lang="lua">instance.Best:SetText( Locale.ToNumber(best[1], "#'%'") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0370}}<syntaxhighlight lang="lua">instance.Average:SetText( Locale.ToNumber( GetAverage( m_ApprovalTable, iPlayer ), "#'%'" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0374}}<syntaxhighlight lang="lua">instance.Worst:LocalizeAndSetText( Locale.ToNumber(worst[1], "#'%'" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0376}}<syntaxhighlight lang="lua">instance.Rank:SetText( Locale.ToNumber(GetRank( m_ApprovalTable, iPlayer ), "#") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0411}}<syntaxhighlight lang="lua">instance.Value:SetText( Locale.ToNumber(m_LiteracyTable[ iPlayer ], "#'%'" ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0423}}<syntaxhighlight lang="lua">instance.Rank:SetText( Locale.ToNumber(GetRank( m_LiteracyTable, iPlayer ), "#") );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0181}}<syntaxhighlight lang="lua">Controls.TotalGoldValue:SetText( Locale.ToNumber( pPlayer:GetGold(), "#.##" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0184}}<syntaxhighlight lang="lua">Controls.NetGoldValue:SetText( Locale.ToNumber( netGPT, "#.##" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0188}}<syntaxhighlight lang="lua">Controls.ScienceLostValue:SetText( Locale.ToNumber( pPlayer:GetScienceFromBudgetDeficitTimes100() / 100, "#.##" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0193}}<syntaxhighlight lang="lua">Controls.GrossGoldValue:SetText( "[COLOR_POSITIVE_TEXT]" .. Locale.ToNumber( pPlayer:CalculateGrossGoldTimes100() / 100, "#.##" ) .. "[ENDCOLOR]" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0195}}<syntaxhighlight lang="lua">Controls.TotalExpenseValue:SetText( "[COLOR_NEGATIVE_TEXT]" .. Locale.ToNumber( pPlayer:CalculateInflatedCosts(), "#.##" ) .. "[ENDCOLOR]" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0198}}<syntaxhighlight lang="lua">Controls.CityIncomeValue:SetText( Locale.ToNumber( pPlayer:GetGoldFromCitiesTimes100() / 100, "#.##" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0212}}<syntaxhighlight lang="lua">instance.TradeIncomeValue:SetText( Locale.ToNumber( CityIncome, "#.##" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0229}}<syntaxhighlight lang="lua">Controls.DiploIncomeValue:SetText( Locale.ToNumber( diploGPT, "#.##" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0234}}<syntaxhighlight lang="lua">Controls.TradeIncomeValue:SetText( Locale.ToNumber( pPlayer:GetCityConnectionGoldTimes100() / 100, "#.##" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0257}}<syntaxhighlight lang="lua">instance.TradeIncomeValue:SetText( Locale.ToNumber( tradeIncome, "#.##" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0287}}<syntaxhighlight lang="lua">local fCostPer = Locale.ToNumber( iTotalUnitMaintenance / iPaidUnits , "#.##" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0318}}<syntaxhighlight lang="lua">Controls.BuildingExpenseValue:SetText( Locale.ToNumber( pPlayer:GetBuildingGoldMaintenance(), "#.##" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0332}}<syntaxhighlight lang="lua">instance.TradeIncomeValue:SetText( Locale.ToNumber( BuildingCost, "#.##" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0359}}<syntaxhighlight lang="lua">Controls.TileExpenseValue:SetText( Locale.ToNumber( pPlayer:GetImprovementGoldMaintenance(), "#.##" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0362}}<syntaxhighlight lang="lua">Controls.DiploExpenseValue:SetText( Locale.ToNumber( pPlayer:GetGoldPerTurnFromDiplomacy(), "#.##" ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0237}}<syntaxhighlight lang="lua">Controls.ReligionIncomeValue:SetText( Locale.ToNumber( religionGPT, "#.##" ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0425}}<syntaxhighlight lang="lua">Controls.TheirStrengthValue:SetText( Locale.ToNumber(iTheirStrength / 100, "#.##") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1432}}<syntaxhighlight lang="lua">Controls.TheirStrengthValue:SetText( Locale.ToNumber(theirUnitStrength / 100, "#.##"));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1438}}<syntaxhighlight lang="lua">Controls.MyStrengthValue:SetText( Locale.ToNumber(myCityStrength / 100, "#.##"));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0222}}<syntaxhighlight lang="lua">instance.TradeIncomeValue:SetText( Locale.ToNumber( resource.Happiness, "#.##" ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0390}}<syntaxhighlight lang="lua">local iUnhappinessFromUnits = Locale.ToNumber( pPlayer:GetUnhappinessFromUnits() / 100, "#.##" );</syntaxhighlight>
{{CodeLine5|0391}}<syntaxhighlight lang="lua">local iUnhappinessFromCityCount = Locale.ToNumber( pPlayer:GetUnhappinessFromCityCount() / 100, "#.##" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0393}}<syntaxhighlight lang="lua">local iUnhappinessFromPop = Locale.ToNumber( pPlayer:GetUnhappinessFromCityPopulation() / 100, "#.##" );</syntaxhighlight>
{{CodeLine5|0394}}<syntaxhighlight lang="lua">local iUnhappinessFromOccupiedCities = Locale.ToNumber( pPlayer:GetUnhappinessFromOccupiedCities() / 100, "#.##" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0576}}<syntaxhighlight lang="lua">instance.TradeIncomeValue:SetText( Locale.ToNumber( fUnhappinessTimes100, "#.##" ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0642}}<syntaxhighlight lang="lua">local iUnhappinessFromPop = Locale.ToNumber( unhappinessFromPop / 100, "#.##" );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ToNumber]]