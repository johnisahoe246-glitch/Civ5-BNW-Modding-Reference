{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


Fired once per turn for each player (not just active/human player). Modder experimentation has found that it is fired at the start of turn; also, it seems not to run for the first turn of the game (for all players), runs only for human player on the second turn, and thereafter it runs for all players. There is no indication as to why this is.


=Usage=
<code>'''void''' GameEvents.PlayerDoTurn<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''The ID of the player whose turn is in question''
|}


=Source code samples=
''Too many occurences. Only 50 out of 5 are listed.''

{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0302}}<syntaxhighlight lang="lua">GameEvents.PlayerDoTurn.Add(function(iPlayer)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0304}}<syntaxhighlight lang="lua">-- Only on first player's turn</syntaxhighlight>
{{CodeLine5|0305}}<syntaxhighlight lang="lua">if (iPlayer > 0) then</syntaxhighlight>
{{CodeLine5|0306}}<syntaxhighlight lang="lua">return false;</syntaxhighlight>
{{CodeLine5|0307}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0309}}<syntaxhighlight lang="lua">--(KLUDGE - using an unused modern era CvGame data field as a counter)</syntaxhighlight>
{{CodeLine5|0310}}<syntaxhighlight lang="lua">local iGenerateTreasureTurn = Game:GetNoNukesCount();</syntaxhighlight>
{{CodeLine5|0311}}<syntaxhighlight lang="lua">local iGameTurn = Game.GetGameTurn();</syntaxhighlight>
{{CodeLine5|0312}}<syntaxhighlight lang="lua">local iFeatureID;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0314}}<syntaxhighlight lang="lua">-- Time to generate a treasure?</syntaxhighlight>
{{CodeLine5|0315}}<syntaxhighlight lang="lua">if (iGameTurn > iGenerateTreasureTurn) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0317}}<syntaxhighlight lang="lua">iFeatureID = GameInfoTypes["FEATURE_EL_DORADO"];</syntaxhighlight>
{{CodeLine5|0318}}<syntaxhighlight lang="lua">SpawnTreasure(iFeatureID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0320}}<syntaxhighlight lang="lua">iFeatureID = GameInfoTypes["FEATURE_POTOSI"];</syntaxhighlight>
{{CodeLine5|0321}}<syntaxhighlight lang="lua">SpawnTreasure(iFeatureID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0323}}<syntaxhighlight lang="lua">-- Reset turn of next treasure generation</syntaxhighlight>
{{CodeLine5|0324}}<syntaxhighlight lang="lua">local iRandom = Game.Rand(20, "Delay between natural wonder treasures");</syntaxhighlight>
{{CodeLine5|0325}}<syntaxhighlight lang="lua">Game:ChangeNoNukesCount(5 + iRandom);</syntaxhighlight>
{{CodeLine5|0326}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0328}}<syntaxhighlight lang="lua">-- AI units on high difficulty</syntaxhighlight>
{{CodeLine5|0329}}<syntaxhighlight lang="lua">local unit;</syntaxhighlight>
{{CodeLine5|0330}}<syntaxhighlight lang="lua">local iHandicap = Game:GetHandicapType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0332}}<syntaxhighlight lang="lua">if (iGameTurn == 10) then</syntaxhighlight>
{{CodeLine5|0333}}<syntaxhighlight lang="lua">for iLoopPlayer = 1, 5, 1 do</syntaxhighlight>
{{CodeLine5|0334}}<syntaxhighlight lang="lua">   local pLoopPlayer = Players[iLoopPlayer];</syntaxhighlight>
{{CodeLine5|0335}}<syntaxhighlight lang="lua">   if (pLoopPlayer:IsAlive() and pLoopPlayer:GetStartingPlot():GetX() > 50) then</syntaxhighlight>
{{CodeLine5|0336}}<syntaxhighlight lang="lua">   if (iHandicap > 5) then</syntaxhighlight>
{{CodeLine5|0337}}<syntaxhighlight lang="lua">   iUnitID = GameInfoTypes["UNIT_SETTLER"];</syntaxhighlight>
{{CodeLine5|0338}}<syntaxhighlight lang="lua">   unit = pLoopPlayer:InitUnit (iUnitID, pLoopPlayer:GetStartingPlot():GetX(), pLoopPlayer:GetStartingPlot():GetY());</syntaxhighlight>
{{CodeLine5|0339}}<syntaxhighlight lang="lua">   unit:JumpToNearestValidPlot();</syntaxhighlight>
{{CodeLine5|0340}}<syntaxhighlight lang="lua">   iUnitID = GameInfoTypes["UNIT_PIKEMAN"];</syntaxhighlight>
{{CodeLine5|0341}}<syntaxhighlight lang="lua">   unit = pLoopPlayer:InitUnit (iUnitID, pLoopPlayer:GetStartingPlot():GetX(), pLoopPlayer:GetStartingPlot():GetY());</syntaxhighlight>
{{CodeLine5|0342}}<syntaxhighlight lang="lua">   unit:JumpToNearestValidPlot();</syntaxhighlight>
{{CodeLine5|0343}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0344}}<syntaxhighlight lang="lua">   if (iHandicap > 6) then</syntaxhighlight>
{{CodeLine5|0345}}<syntaxhighlight lang="lua">   iUnitID = GameInfoTypes["UNIT_CARAVEL"];</syntaxhighlight>
{{CodeLine5|0346}}<syntaxhighlight lang="lua">   unit = pLoopPlayer:InitUnit (iUnitID, pLoopPlayer:GetStartingPlot():GetX(), pLoopPlayer:GetStartingPlot():GetY(), GameInfoTypes.UNITAI_EXPLORE_SEA, DirectionTypes.DIRECTION_WEST);</syntaxhighlight>
{{CodeLine5|0347}}<syntaxhighlight lang="lua">   unit:JumpToNearestValidPlot();</syntaxhighlight>
{{CodeLine5|0348}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0349}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0350}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0351}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0353}}<syntaxhighlight lang="lua">   if (iGameTurn == 15) then</syntaxhighlight>
{{CodeLine5|0354}}<syntaxhighlight lang="lua">   for iLoopPlayer = 1, 5, 1 do</syntaxhighlight>
{{CodeLine5|0355}}<syntaxhighlight lang="lua">   local pLoopPlayer = Players[iLoopPlayer];</syntaxhighlight>
{{CodeLine5|0356}}<syntaxhighlight lang="lua">   if (pLoopPlayer:IsAlive()and pLoopPlayer:GetStartingPlot():GetX() > 50) then</syntaxhighlight>
{{CodeLine5|0357}}<syntaxhighlight lang="lua">   if (iHandicap > 6) then</syntaxhighlight>
{{CodeLine5|0358}}<syntaxhighlight lang="lua">   iUnitID = GameInfoTypes["UNIT_SETTLER"];</syntaxhighlight>
{{CodeLine5|0359}}<syntaxhighlight lang="lua">   unit = pLoopPlayer:InitUnit (iUnitID, pLoopPlayer:GetStartingPlot():GetX(), pLoopPlayer:GetStartingPlot():GetY());</syntaxhighlight>
{{CodeLine5|0360}}<syntaxhighlight lang="lua">   unit:JumpToNearestValidPlot();</syntaxhighlight>
{{CodeLine5|0361}}<syntaxhighlight lang="lua">   iUnitID = GameInfoTypes["UNIT_PIKEMAN"];</syntaxhighlight>
{{CodeLine5|0362}}<syntaxhighlight lang="lua">   unit = pLoopPlayer:InitUnit (iUnitID, pLoopPlayer:GetStartingPlot():GetX(), pLoopPlayer:GetStartingPlot():GetY());</syntaxhighlight>
{{CodeLine5|0363}}<syntaxhighlight lang="lua">   unit:JumpToNearestValidPlot();</syntaxhighlight>
{{CodeLine5|0364}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0365}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0366}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0367}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0369}}<syntaxhighlight lang="lua">   if (iGameTurn == 20) then</syntaxhighlight>
{{CodeLine5|0370}}<syntaxhighlight lang="lua">   for iLoopPlayer = 1, 5, 1 do</syntaxhighlight>
{{CodeLine5|0371}}<syntaxhighlight lang="lua">   local pLoopPlayer = Players[iLoopPlayer];</syntaxhighlight>
{{CodeLine5|0372}}<syntaxhighlight lang="lua">   if (pLoopPlayer:IsAlive() and pLoopPlayer:GetStartingPlot():GetX() > 50) then</syntaxhighlight>
{{CodeLine5|0373}}<syntaxhighlight lang="lua">   if (iHandicap > 3) then</syntaxhighlight>
{{CodeLine5|0374}}<syntaxhighlight lang="lua">   iUnitID = GameInfoTypes["UNIT_SETTLER"];</syntaxhighlight>
{{CodeLine5|0375}}<syntaxhighlight lang="lua">   unit = pLoopPlayer:InitUnit (iUnitID, pLoopPlayer:GetStartingPlot():GetX(), pLoopPlayer:GetStartingPlot():GetY());</syntaxhighlight>
{{CodeLine5|0376}}<syntaxhighlight lang="lua">   unit:JumpToNearestValidPlot();</syntaxhighlight>
{{CodeLine5|0377}}<syntaxhighlight lang="lua">   iUnitID = GameInfoTypes["UNIT_PIKEMAN"];</syntaxhighlight>
{{CodeLine5|0378}}<syntaxhighlight lang="lua">   unit = pLoopPlayer:InitUnit (iUnitID, pLoopPlayer:GetStartingPlot():GetX(), pLoopPlayer:GetStartingPlot():GetY());</syntaxhighlight>
{{CodeLine5|0379}}<syntaxhighlight lang="lua">   unit:JumpToNearestValidPlot();</syntaxhighlight>
{{CodeLine5|0380}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0381}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0382}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0383}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0385}}<syntaxhighlight lang="lua">   return false;</syntaxhighlight>
{{CodeLine5|0386}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0222}}<syntaxhighlight lang="lua">GameEvents.PlayerDoTurn.Add(function(iPlayer)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0224}}<syntaxhighlight lang="lua">-- Only on first player's turn</syntaxhighlight>
{{CodeLine5|0225}}<syntaxhighlight lang="lua">if (iPlayer > 0) then</syntaxhighlight>
{{CodeLine5|0226}}<syntaxhighlight lang="lua">return false;</syntaxhighlight>
{{CodeLine5|0227}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0230}}<syntaxhighlight lang="lua">local savedData = Modding.OpenSaveData();</syntaxhighlight>
{{CodeLine5|0231}}<syntaxhighlight lang="lua">local iValue = savedData.GetValue("TurnsBetweenBonuses");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0233}}<syntaxhighlight lang="lua">if (iValue ~= nil) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0235}}<syntaxhighlight lang="lua">local iTemp = math.floor(Game.GetGameTurn() / iValue);</syntaxhighlight>
{{CodeLine5|0236}}<syntaxhighlight lang="lua">if (Game.GetGameTurn() > 0 and Game.GetGameTurn()< 51 and iTemp * iValue == Game.GetGameTurn()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0238}}<syntaxhighlight lang="lua">for iPlayer = 0, 3, 1 do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0240}}<syntaxhighlight lang="lua">   local pPlayer = Players[iPlayer];</syntaxhighlight>
{{CodeLine5|0241}}<syntaxhighlight lang="lua">   local playerStartPlot = pPlayer:GetStartingPlot();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0243}}<syntaxhighlight lang="lua">   -- Anglo-Saxon England?</syntaxhighlight>
{{CodeLine5|0244}}<syntaxhighlight lang="lua">   if (playerStartPlot:GetX() == 43 and playerStartPlot:GetY() == 17) then</syntaxhighlight>
{{CodeLine5|0245}}<syntaxhighlight lang="lua">   CollectTaxes(iPlayer);</syntaxhighlight>
{{CodeLine5|0246}}<syntaxhighlight lang="lua">   else</syntaxhighlight>
{{CodeLine5|0247}}<syntaxhighlight lang="lua">   NewRecruits(iPlayer);</syntaxhighlight>
{{CodeLine5|0248}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0249}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0250}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0251}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0252}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0498}}<syntaxhighlight lang="lua">GameEvents.PlayerDoTurn.Add(function(iPlayer)</syntaxhighlight>
{{CodeLine5|0499}}<syntaxhighlight lang="lua">local iTurn = Game.GetGameTurn();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0501}}<syntaxhighlight lang="lua">-- Update on Barbarian player's turn (after all major civs take their turn) so that we are fair to all players</syntaxhighlight>
{{CodeLine5|0502}}<syntaxhighlight lang="lua">if (iPlayer == 63) then</syntaxhighlight>
{{CodeLine5|0503}}<syntaxhighlight lang="lua">UpdateMostAdvancedUnits();</syntaxhighlight>
{{CodeLine5|0504}}<syntaxhighlight lang="lua">UpdatePlayerStatus();</syntaxhighlight>
{{CodeLine5|0505}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0507}}<syntaxhighlight lang="lua">return false;</syntaxhighlight>
{{CodeLine5|0508}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">GameEvents.PlayerDoTurn.Add(function(iPlayer)</syntaxhighlight>
{{CodeLine5|0145}}<syntaxhighlight lang="lua">local iReformationTurn = GetPersistentProperty("ReformationStart");</syntaxhighlight>
{{CodeLine5|0146}}<syntaxhighlight lang="lua">local iTurn = Game.GetGameTurn();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0148}}<syntaxhighlight lang="lua">-- Only on first player's turn</syntaxhighlight>
{{CodeLine5|0149}}<syntaxhighlight lang="lua">if (iPlayer > 0 or iTurn < 1) then</syntaxhighlight>
{{CodeLine5|0150}}<syntaxhighlight lang="lua">return false;</syntaxhighlight>
{{CodeLine5|0151}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">if (iReformationTurn > -1) then</syntaxhighlight>
{{CodeLine5|0154}}<syntaxhighlight lang="lua">if (iReformationTurn == iTurn) then</syntaxhighlight>
{{CodeLine5|0155}}<syntaxhighlight lang="lua">StartReformation();</syntaxhighlight>
{{CodeLine5|0156}}<syntaxhighlight lang="lua">elseif (GetPersistentProperty("SecondReformer") == iTurn) then</syntaxhighlight>
{{CodeLine5|0157}}<syntaxhighlight lang="lua">ReformationPhaseTwo();</syntaxhighlight>
{{CodeLine5|0158}}<syntaxhighlight lang="lua">elseif (GetPersistentProperty("ThirdReformer") == iTurn) then</syntaxhighlight>
{{CodeLine5|0159}}<syntaxhighlight lang="lua">ReformationPhaseThree();</syntaxhighlight>
{{CodeLine5|0160}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0161}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0162}}<syntaxhighlight lang="lua">if (Game.GetGameTurnYear() > 1514) then</syntaxhighlight>
{{CodeLine5|0163}}<syntaxhighlight lang="lua">SetPersistentProperty("ReformationStart", iTurn + 1);</syntaxhighlight>
{{CodeLine5|0164}}<syntaxhighlight lang="lua">SetPersistentProperty("SecondReformer", iTurn + 4);</syntaxhighlight>
{{CodeLine5|0165}}<syntaxhighlight lang="lua">SetPersistentProperty("ThirdReformer", iTurn + 7);</syntaxhighlight>
{{CodeLine5|0166}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0167}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0169}}<syntaxhighlight lang="lua">ScoreHolyCities();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0171}}<syntaxhighlight lang="lua">if (iTurn == 40) then</syntaxhighlight>
{{CodeLine5|0172}}<syntaxhighlight lang="lua">BringInMongols();</syntaxhighlight>
{{CodeLine5|0173}}<syntaxhighlight lang="lua">elseif (iTurn == 50 or iTurn == 60 or iTurn == 70 or iTurn == 85 or iTurn == 110) then</syntaxhighlight>
{{CodeLine5|0174}}<syntaxhighlight lang="lua">ReinforceMongols();</syntaxhighlight>
{{CodeLine5|0175}}<syntaxhighlight lang="lua">elseif (iTurn == 150) then</syntaxhighlight>
{{CodeLine5|0176}}<syntaxhighlight lang="lua">MongolsPullOut();</syntaxhighlight>
{{CodeLine5|0177}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0179}}<syntaxhighlight lang="lua">return false;</syntaxhighlight>
{{CodeLine5|0180}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0233}}<syntaxhighlight lang="lua">GameEvents.PlayerDoTurn.Add(function(iPlayer)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0235}}<syntaxhighlight lang="lua">--if (iPlayer ~= nil) then</syntaxhighlight>
{{CodeLine5|0236}}<syntaxhighlight lang="lua">--   print("GameEvents.PlayerDoTurn.Add, iPlayer: " .. iPlayer);</syntaxhighlight>
{{CodeLine5|0237}}<syntaxhighlight lang="lua">--else</syntaxhighlight>
{{CodeLine5|0238}}<syntaxhighlight lang="lua">--   print("GameEvents.PlayerDoTurn.Add, iPlayer: nil");</syntaxhighlight>
{{CodeLine5|0239}}<syntaxhighlight lang="lua">--end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0241}}<syntaxhighlight lang="lua">local savedData = Modding.OpenSaveData();</syntaxhighlight>
{{CodeLine5|0242}}<syntaxhighlight lang="lua">local iCitiesCaptured = 0;</syntaxhighlight>
{{CodeLine5|0243}}<syntaxhighlight lang="lua">if (IsWesternRoman(iPlayer)) then</syntaxhighlight>
{{CodeLine5|0244}}<syntaxhighlight lang="lua">iCitiesCaptured = savedData.GetValue("WesternRomeCitiesCaptured");</syntaxhighlight>
{{CodeLine5|0245}}<syntaxhighlight lang="lua">savedData.SetValue("WesternRomeCitiesCaptured", 0);</syntaxhighlight>
{{CodeLine5|0246}}<syntaxhighlight lang="lua">elseif (IsEasternRoman(iPlayer)) then</syntaxhighlight>
{{CodeLine5|0247}}<syntaxhighlight lang="lua">iCitiesCaptured = savedData.GetValue("EasternRomeCitiesCaptured")</syntaxhighlight>
{{CodeLine5|0248}}<syntaxhighlight lang="lua">savedData.SetValue("EasternRomeCitiesCaptured", 0);</syntaxhighlight>
{{CodeLine5|0249}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0251}}<syntaxhighlight lang="lua">print("GameEvents.PlayerDoTurn.Add, iCitiesCaptured: " .. iCitiesCaptured);</syntaxhighlight>
{{CodeLine5|0252}}<syntaxhighlight lang="lua">if (iCitiesCaptured > 0) then</syntaxhighlight>
{{CodeLine5|0253}}<syntaxhighlight lang="lua">print("GameEvents.PlayerDoTurn.Add, rewarding culture");</syntaxhighlight>
{{CodeLine5|0254}}<syntaxhighlight lang="lua">Players[iPlayer]:ChangeJONSCulture(20 * iCitiesCaptured);</syntaxhighlight>
{{CodeLine5|0255}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0257}}<syntaxhighlight lang="lua">if (Players[iPlayer]:HasPolicy(GameInfo.Policies["POLICY_BARBARIAN_FINISHER"].ID)) then</syntaxhighlight>
{{CodeLine5|0258}}<syntaxhighlight lang="lua">if (Players[iPlayer]:GetJONSCulture() > 0) then</syntaxhighlight>
{{CodeLine5|0259}}<syntaxhighlight lang="lua">local iDiv = Players[iPlayer]:GetJONSCulture() / 3;</syntaxhighlight>
{{CodeLine5|0260}}<syntaxhighlight lang="lua">local iMod = Players[iPlayer]:GetJONSCulture() % 3;</syntaxhighlight>
{{CodeLine5|0261}}<syntaxhighlight lang="lua">Players[iPlayer]:ChangeGold(iDiv);</syntaxhighlight>
{{CodeLine5|0262}}<syntaxhighlight lang="lua">Players[iPlayer]:SetJONSCulture(iMod);</syntaxhighlight>
{{CodeLine5|0263}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0264}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0266}}<syntaxhighlight lang="lua">if (Players[iPlayer]:HasPolicy(GameInfo.Policies["POLICY_SASSANID_FINISHER"].ID)) then</syntaxhighlight>
{{CodeLine5|0267}}<syntaxhighlight lang="lua">if (Players[iPlayer]:GetJONSCulture() > 0) then</syntaxhighlight>
{{CodeLine5|0268}}<syntaxhighlight lang="lua">local iDiv = Players[iPlayer]:GetJONSCulture() / 3;</syntaxhighlight>
{{CodeLine5|0269}}<syntaxhighlight lang="lua">local iMod = Players[iPlayer]:GetJONSCulture() % 3;</syntaxhighlight>
{{CodeLine5|0270}}<syntaxhighlight lang="lua">Players[iPlayer]:ChangeGold(iDiv);</syntaxhighlight>
{{CodeLine5|0271}}<syntaxhighlight lang="lua">Players[iPlayer]:SetJONSCulture(iMod);</syntaxhighlight>
{{CodeLine5|0272}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0273}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0275}}<syntaxhighlight lang="lua">-- Only on first player's turn</syntaxhighlight>
{{CodeLine5|0276}}<syntaxhighlight lang="lua">if (iPlayer > 0) then</syntaxhighlight>
{{CodeLine5|0277}}<syntaxhighlight lang="lua">return false;</syntaxhighlight>
{{CodeLine5|0278}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0280}}<syntaxhighlight lang="lua">--print("PlayerDoTurn");</syntaxhighlight>
{{CodeLine5|0281}}<syntaxhighlight lang="lua">--print(iPlayer);</syntaxhighlight>
{{CodeLine5|0282}}<syntaxhighlight lang="lua">--local playerStartPlot = Players[iPlayer]:GetStartingPlot();</syntaxhighlight>
{{CodeLine5|0283}}<syntaxhighlight lang="lua">--print(playerStartPlot:GetX());</syntaxhighlight>
{{CodeLine5|0284}}<syntaxhighlight lang="lua">--print(playerStartPlot:GetY());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0286}}<syntaxhighlight lang="lua">for iPlayerLoop = 0, GameDefines.MAX_MAJOR_CIVS-1, 1 do</syntaxhighlight>
{{CodeLine5|0287}}<syntaxhighlight lang="lua">   local pPlayer = Players[iPlayerLoop];</syntaxhighlight>
{{CodeLine5|0288}}<syntaxhighlight lang="lua">   if (pPlayer:IsAlive() and IsEmpire(iPlayerLoop)) then</syntaxhighlight>
{{CodeLine5|0289}}<syntaxhighlight lang="lua">   local iScore = 0;</syntaxhighlight>
{{CodeLine5|0290}}<syntaxhighlight lang="lua">   for pCity in pPlayer:Cities() do</syntaxhighlight>
{{CodeLine5|0291}}<syntaxhighlight lang="lua">   local iOriginalOwner = pCity:GetOriginalOwner();</syntaxhighlight>
{{CodeLine5|0292}}<syntaxhighlight lang="lua">   -- if city owner is an empire and the original owner was an empire</syntaxhighlight>
{{CodeLine5|0293}}<syntaxhighlight lang="lua">   if (IsEmpire(iOriginalOwner)) then</syntaxhighlight>
{{CodeLine5|0294}}<syntaxhighlight lang="lua">   --   then give points according to how large the city is</syntaxhighlight>
{{CodeLine5|0295}}<syntaxhighlight lang="lua">   iScore = iScore + pCity:GetPopulation();</syntaxhighlight>
{{CodeLine5|0296}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0297}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0299}}<syntaxhighlight lang="lua">   if (IsRoman(iPlayerLoop)) then</syntaxhighlight>
{{CodeLine5|0300}}<syntaxhighlight lang="lua">   iScore = iScore / 2;</syntaxhighlight>
{{CodeLine5|0301}}<syntaxhighlight lang="lua">   elseif (IsSassanid(iPlayerLoop)) then</syntaxhighlight>
{{CodeLine5|0302}}<syntaxhighlight lang="lua">   iScore = (4 * iScore) / 3;</syntaxhighlight>
{{CodeLine5|0303}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0305}}<syntaxhighlight lang="lua">   pPlayer:ChangeScoreFromTechs(iScore);</syntaxhighlight>
{{CodeLine5|0306}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0307}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0310}}<syntaxhighlight lang="lua">   if (iCitiesCaptured > 0) then</syntaxhighlight>
{{CodeLine5|0311}}<syntaxhighlight lang="lua">   --print("Doing city popup");</syntaxhighlight>
{{CodeLine5|0312}}<syntaxhighlight lang="lua">   local popupInfo = {</syntaxhighlight>
{{CodeLine5|0313}}<syntaxhighlight lang="lua">   Data1 = 500,</syntaxhighlight>
{{CodeLine5|0314}}<syntaxhighlight lang="lua">   Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0315}}<syntaxhighlight lang="lua">   }</syntaxhighlight>
{{CodeLine5|0316}}<syntaxhighlight lang="lua">   popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_FOR_SCENARIO_ROMAN_CITY_CAPTURE_CULTURE", iCitiesCaptured, iCitiesCaptured * 20);</syntaxhighlight>
{{CodeLine5|0317}}<syntaxhighlight lang="lua">   UI.AddPopup(popupInfo);</syntaxhighlight>
{{CodeLine5|0318}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0321}}<syntaxhighlight lang="lua">   --if (not IsEmpire(iPlayer)) then</syntaxhighlight>
{{CodeLine5|0322}}<syntaxhighlight lang="lua">   --return false;</syntaxhighlight>
{{CodeLine5|0323}}<syntaxhighlight lang="lua">   --end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0325}}<syntaxhighlight lang="lua">   --local pPlayer = Players[iPlayer];</syntaxhighlight>
{{CodeLine5|0326}}<syntaxhighlight lang="lua">   --for pCity in pPlayer:Cities() do</syntaxhighlight>
{{CodeLine5|0327}}<syntaxhighlight lang="lua">   --local iOriginalOwner = pCity:GetOriginalOwner();</syntaxhighlight>
{{CodeLine5|0328}}<syntaxhighlight lang="lua">   ---- if city owner is an empire and the original owner was an empire</syntaxhighlight>
{{CodeLine5|0329}}<syntaxhighlight lang="lua">   --if (IsEmpire(iOriginalOwner)) then</syntaxhighlight>
{{CodeLine5|0330}}<syntaxhighlight lang="lua">   ----   then give points according to how large the city is</syntaxhighlight>
{{CodeLine5|0331}}<syntaxhighlight lang="lua">   --pPlayer:ChangeScoreFromTechs(pCity:GetPopulation());</syntaxhighlight>
{{CodeLine5|0332}}<syntaxhighlight lang="lua">   --end</syntaxhighlight>
{{CodeLine5|0333}}<syntaxhighlight lang="lua">   --end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0335}}<syntaxhighlight lang="lua">   return false;</syntaxhighlight>
{{CodeLine5|0336}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlayerDoTurn]]
[[Category:Civ5 Players API|PlayerDoTurn]]