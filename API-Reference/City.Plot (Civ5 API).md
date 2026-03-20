{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|Plot}} City:Plot<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0130}}<syntaxhighlight lang="lua">UI.LookAt(pCity:Plot(), 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AnnexCityPopup.lua}}
:<code>UI/InGame/PopupsGeneric/AnnexCityPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0035}}<syntaxhighlight lang="lua">UI.DoSelectCityAtPlot( newCity:Plot() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0024}}<syntaxhighlight lang="lua">thisPlot = pHeadSelectedCity:Plot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1070}}<syntaxhighlight lang="lua">UI.HighlightCanPlacePlots(unit, city:Plot());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0781}}<syntaxhighlight lang="lua">local pPlot = pCity:Plot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0293}}<syntaxhighlight lang="lua">lastCityEnteredPlot = lastCityEntered:Plot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0197}}<syntaxhighlight lang="lua">local plot = city:Plot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0816}}<syntaxhighlight lang="lua">pJerusalemPlot = pCity:Plot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0822}}<syntaxhighlight lang="lua">pVaticanPlot = pCity:Plot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0830}}<syntaxhighlight lang="lua">pMeccaPlot = pCity:Plot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0876}}<syntaxhighlight lang="lua">pByzantinePlot = capital:Plot();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1075}}<syntaxhighlight lang="lua">local pCapitalCityPlot = pCapitalCity:Plot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1941}}<syntaxhighlight lang="lua">return v:Plot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2525}}<syntaxhighlight lang="lua">local pPlot = v:Plot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2923}}<syntaxhighlight lang="lua">return pCity:Plot();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Plot]]