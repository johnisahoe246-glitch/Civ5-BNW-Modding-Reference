{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetPopulation<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0244}}<syntaxhighlight lang="lua">local cityPopulation = math.floor(city:GetPopulation());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0163}}<syntaxhighlight lang="lua">sortEntry.Population = pCity:GetPopulation();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0751}}<syntaxhighlight lang="lua">local cityPopulation = math.floor(pCity:GetPopulation());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0259}}<syntaxhighlight lang="lua">local strPopInfo = " (" .. pCity:GetPopulation() .. ")";</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0401}}<syntaxhighlight lang="lua">iOccupiedPop = iOccupiedPop + pCity:GetPopulation();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0612}}<syntaxhighlight lang="lua">iYieldPerPop = iYieldPerPop * pCity:GetPopulation();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0680}}<syntaxhighlight lang="lua">local iYieldFromPop = iYieldPerPop * pCity:GetPopulation();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0206}}<syntaxhighlight lang="lua">local cityPopulation = city:GetPopulation();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2471}}<syntaxhighlight lang="lua">instance.CityPop:SetText( pCity:GetPopulation() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0295}}<syntaxhighlight lang="lua">iScore = iScore + pCity:GetPopulation();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0318}}<syntaxhighlight lang="lua">if (pCity:GetPopulation() > iBestPop) then</syntaxhighlight>
{{CodeLine5|0319}}<syntaxhighlight lang="lua">iBestPop = pCity:GetPopulation();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2751}}<syntaxhighlight lang="lua">if (v:GetPopulation() >= 3) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPopulation]]
[[Category:Civ5 Food & Population API|GetPopulation]]