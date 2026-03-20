{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:DestroyAllChildren<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChooseFaithGreatPerson.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseFaithGreatPerson.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0022}}<syntaxhighlight lang="lua">stackControl:DestroyAllChildren();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">Controls.MainStack:DestroyAllChildren();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">Controls.CurrentDealsStack:DestroyAllChildren();</syntaxhighlight>
{{CodeLine5|0016}}<syntaxhighlight lang="lua">Controls.HistoricDealsStack:DestroyAllChildren();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0025}}<syntaxhighlight lang="lua">Controls.ItemStack:DestroyAllChildren();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0201}}<syntaxhighlight lang="lua">Controls.CityStack:DestroyAllChildren();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0245}}<syntaxhighlight lang="lua">Controls.TradeStack:DestroyAllChildren();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0321}}<syntaxhighlight lang="lua">Controls.BuildingsStack:DestroyAllChildren();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0141}}<syntaxhighlight lang="lua">Controls.SelectCivStack:DestroyAllChildren();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">Controls.LuxuryHappinessStack:DestroyAllChildren();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0266}}<syntaxhighlight lang="lua">Controls.CityBuildingStack:DestroyAllChildren();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0298}}<syntaxhighlight lang="lua">Controls.TradeRouteStack:DestroyAllChildren();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0332}}<syntaxhighlight lang="lua">Controls.GarrisonStack:DestroyAllChildren();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0560}}<syntaxhighlight lang="lua">Controls.CityUnhappinessStack:DestroyAllChildren();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0611}}<syntaxhighlight lang="lua">Controls.ResourcesAvailableStack:DestroyAllChildren();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0654}}<syntaxhighlight lang="lua">Controls.ResourcesImportedStack:DestroyAllChildren();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0696}}<syntaxhighlight lang="lua">Controls.ResourcesExportedStack:DestroyAllChildren();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0737}}<syntaxhighlight lang="lua">Controls.ResourcesLocalStack:DestroyAllChildren();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0326}}<syntaxhighlight lang="lua">Controls.LocalCityStack:DestroyAllChildren();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0034}}<syntaxhighlight lang="lua">Controls.Stack:DestroyAllChildren();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0844}}<syntaxhighlight lang="lua">Controls.ChatStack:DestroyAllChildren();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DestroyAllChildren]]