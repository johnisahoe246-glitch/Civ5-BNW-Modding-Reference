{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|CityID}} City:GetID<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0392}}<syntaxhighlight lang="lua">controls.CityBannerProductionButton:SetVoids( city:GetID(), nil );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1252}}<syntaxhighlight lang="lua">OnCityCreated( ToHexFromGrid( Vector2( city:GetX(), city:GetY() ) ), player:GetID(), city:GetID() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0426}}<syntaxhighlight lang="lua">instance.ProdButton:SetVoids( city:GetID(), nil );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0229}}<syntaxhighlight lang="lua">Network.SendDoTask(pCity:GetID(), TaskTypes.TASK_CHANGE_WORKING_PLOT, 0, -1, false, bAlt, bShift, bCtrl);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">Data1 = UI.GetHeadSelectedCity():GetID(),</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1670}}<syntaxhighlight lang="lua">Network.SendUpdateCityCitizens(pCity:GetID());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1685}}<syntaxhighlight lang="lua">Network.SendDoTask(pCity:GetID(), TaskTypes.TASK_CHANGE_WORKING_PLOT, iPlotIndex, -1, false, bAlt, bShift, bCtrl);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1698}}<syntaxhighlight lang="lua">Network.SendCityBuyPlot(pHeadSelectedCity:GetID(), plotX, plotY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1769}}<syntaxhighlight lang="lua">elseif ( plot:GetWorkingCity():GetID() ~= pCity:GetID() and  plot:GetWorkingCity():IsWorkingPlot( plot ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1805}}<syntaxhighlight lang="lua">elseif ( pCity:CanWork( plot ) or plot:GetWorkingCity():GetID() ~= pCity:GetID() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1894}}<syntaxhighlight lang="lua">local cityID = city:GetID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2171}}<syntaxhighlight lang="lua">Data1 = pCity:GetID(),</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2189}}<syntaxhighlight lang="lua">Network.SendDoTask(pCity:GetID(), TaskTypes.TASK_UNRAZE, -1, -1, false, false, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2266}}<syntaxhighlight lang="lua">Network.SendSetCityAIFocus( pCity:GetID(), focus );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2294}}<syntaxhighlight lang="lua">Network.SendSetCityAvoidGrowth( pCity:GetID(), not pCity:IsForcedAvoidGrowth() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2375}}<syntaxhighlight lang="lua">Network.SendSellBuilding(pCity:GetID(), g_iBuildingToSell);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameplayUtils.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/GameplayUtils.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0251}}<syntaxhighlight lang="lua">iCityID = pCity:GetID();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">sortEntry.cityID = pCity:GetID();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0191}}<syntaxhighlight lang="lua">local selectedCityID = selectedCity and selectedCity:GetID() or -1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0807}}<syntaxhighlight lang="lua">local currentCityID = city:GetID();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0113}}<syntaxhighlight lang="lua">print("purchase: "..iData.." ; "..city:GetID().." ; "..eYield);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCityName.lua}}
:<code>UI/InGame/Popups/SetCityName.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">Network.SendRenameCity(pCity:GetID(), Controls.EditCityName:GetText());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2465}}<syntaxhighlight lang="lua">local iCityID = pCity:GetID();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0490}}<syntaxhighlight lang="lua">Events.SpecificCityInfoDirty( activePlayerID, pHeadSelectedCity:GetID(), CityUpdateTypes.CITY_UPDATE_TYPE_BANNER);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetID]]