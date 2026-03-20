{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|ResourceType}} City:GetX<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0025}}<syntaxhighlight lang="lua">thisX = pHeadSelectedCity:GetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1252}}<syntaxhighlight lang="lua">OnCityCreated( ToHexFromGrid( Vector2( city:GetX(), city:GetY() ) ), player:GetID(), city:GetID() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0109}}<syntaxhighlight lang="lua">local cityX = city:GetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0107}}<syntaxhighlight lang="lua">instance.Button:SetVoids( pCity:GetX(), pCity:GetY() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0290}}<syntaxhighlight lang="lua">local thisX = pCapital:GetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0956}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay( YieldDisplayTypes.CITY_OWNED, pCity:GetX(), pCity:GetY() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0961}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay( YieldDisplayTypes.CITY_WORKED, pCity:GetX(), pCity:GetY() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1832}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay( YieldDisplayTypes.CITY_PURCHASABLE, pCity:GetX(), pCity:GetY() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0931}}<syntaxhighlight lang="lua">local plotDistance = Map.PlotDistance(pCapital:GetX(), pCapital:GetY(), pMyUnit:GetX(), pMyUnit:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1480}}<syntaxhighlight lang="lua">local plotDistance = Map.PlotDistance(pCapital:GetX(), pCapital:GetY(), pTheirUnit:GetX(), pTheirUnit:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1821}}<syntaxhighlight lang="lua">local plotDistance = Map.PlotDistance(pCapital:GetX(), pCapital:GetY(), theirUnit:GetX(), theirUnit:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0294}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay( YieldDisplayTypes.CITY_WORKED, lastCityEntered:GetX(), lastCityEntered:GetY() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0677}}<syntaxhighlight lang="lua">local iCityStateX = pCityStateCity:GetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0224}}<syntaxhighlight lang="lua">Controls.CityButton:SetVoids( city:GetX(), city:GetY() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1268}}<syntaxhighlight lang="lua">if( g_Deal:IsPossibleToTradeItem( g_iUs, g_iThem, TradeableItems.TRADE_ITEM_CITIES, pCity:GetX(), pCity:GetY() ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1286}}<syntaxhighlight lang="lua">if( g_Deal:IsPossibleToTradeItem( g_iThem, g_iUs, TradeableItems.TRADE_ITEM_CITIES, pCity:GetX(), pCity:GetY() ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2467}}<syntaxhighlight lang="lua">if ( g_Deal:IsPossibleToTradeItem( m_iFrom, m_iTo, TradeableItems.TRADE_ITEM_CITIES, pCity:GetX(), pCity:GetY() ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">if (capital ~= nil and capital:GetX() == iX and capital:GetY() == iY) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">if(capital:GetX() > 50) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0109}}<syntaxhighlight lang="lua">if (Map.PlotDistance(pCity:GetX(), pCity:GetY(), iLondonX, iLondonY) < 8) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">if (pCity:GetX() ~= iLondonX or pCity:GetY() ~= iLondonY) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0415}}<syntaxhighlight lang="lua">if ((pCity:GetX() == 33 and pCity:GetY() == 31) or (pCity:GetX() == 58 and pCity:GetY() == 29)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0428}}<syntaxhighlight lang="lua">local iX = pTargetCity:GetX() + 1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0491}}<syntaxhighlight lang="lua">print(iPlayerLoop .. " " .. pCity:GetX() .. " " .. pCity:GetY());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1060}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit (iUnitID, capital:GetX(), capital:GetY(), UNITAI_WORKER, DirectionTypes.DIRECTION_EAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1064}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit (iUnitID, capital:GetX(), capital:GetY(), UNITAI_DEFENSE, DirectionTypes.DIRECTION_EAST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1264}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit (iUnitID, capital:GetX(), capital:GetY(), UNITAI_SETTLE, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1276}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit (iUnitID, capital:GetX(), capital:GetY(), UNITAI_WORKER, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1288}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit (iUnitID, capital:GetX(), capital:GetY(), UNITAI_DEFENSE, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1300}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit (iUnitID, capital:GetX(), capital:GetY(), UNITAI_GENERAL, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1304}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit (iUnitID, capital:GetX(), capital:GetY(), UNITAI_RANGED, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1566}}<syntaxhighlight lang="lua">elseif (pCity:GetX() == zurichX and pCity:GetY() == zurichY) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1568}}<syntaxhighlight lang="lua">elseif (pCity:GetX() == genevaX and pCity:GetY() == genevaY) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1587}}<syntaxhighlight lang="lua">if (Map.PlotDistance(pReformerCity:GetX(), pReformerCity:GetY(), pCity:GetX(), pCity:GetY()) <= 10) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1612}}<syntaxhighlight lang="lua">unit = pPlayer:InitUnit (iUnitID, capital:GetX(), capital:GetY(), UNITAI_SETTLE, DirectionTypes.DIRECTION_EAST);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetX]]