{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


Triggered whenever any unit moves by any means, for every tile they move into. This includes units that are being created. Note that this event fires before animations are completed.


=Usage=
<code>'''void''' GameEvents.UnitSetXY<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unit, '''int''' x, '''int''' y<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''The ID of the player the unit belongs to.''
|-
|valign="top" style="padding-right:6px;"|unit:
|valign="top"| ''The ID of the unit.''
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''The location of the plot the unit has moved into.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|}

To kill the unit (UnitID) on this event, use unit:Kill(true, -1) to initiate a delayed death. Otherwise the game will crash.--[[User:Killmeplease|Killmeplease]] ([[User talk:Killmeplease|talk]]) 04:16, 1 November 2015 (UTC)

=Source code samples=
''Too many occurences. Only 50 out of 3 are listed.''

{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0130}}<syntaxhighlight lang="lua">GameEvents.UnitSetXY.Add(function(iPlayer, iUnitID, iX, iY)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">local plot = Map.GetPlot(iX, iY);</syntaxhighlight>
{{CodeLine5|0133}}<syntaxhighlight lang="lua">local player = Players[iPlayer];</syntaxhighlight>
{{CodeLine5|0134}}<syntaxhighlight lang="lua">local unit = player:GetUnitByID(iUnitID);</syntaxhighlight>
{{CodeLine5|0135}}<syntaxhighlight lang="lua">if (unit == nil or unit:IsDelayedDeath()) then</syntaxhighlight>
{{CodeLine5|0136}}<syntaxhighlight lang="lua">return false;</syntaxhighlight>
{{CodeLine5|0137}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0139}}<syntaxhighlight lang="lua">-- Caravel that has reached China?</syntaxhighlight>
{{CodeLine5|0140}}<syntaxhighlight lang="lua">if (unit:GetUnitType() == GameInfoTypes["UNIT_CARAVEL"]) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0142}}<syntaxhighlight lang="lua">-- Adjacent to plot owned by China?</syntaxhighlight>
{{CodeLine5|0143}}<syntaxhighlight lang="lua">local bAdjacentChina = IsAdjacentToChina (iX, iY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0145}}<syntaxhighlight lang="lua">if (bAdjacentChina and not player:IsMinorCiv() and not player:IsBarbarian()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0147}}<syntaxhighlight lang="lua">if(iPlayer == Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeLine5|0148}}<syntaxhighlight lang="lua">UI.UnlockAchievement("ACHIEVEMENT_SCENARIO_02_ROUTE_TO_ORIENT");</syntaxhighlight>
{{CodeLine5|0149}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0151}}<syntaxhighlight lang="lua">-- How many have already been? (KLUDGE - using an unused modern era CvGame data field as a counter)</syntaxhighlight>
{{CodeLine5|0152}}<syntaxhighlight lang="lua">local iTotalCircumnavigators = Game:GetNukesExploded();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">if (iTotalCircumnavigators < 3) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0156}}<syntaxhighlight lang="lua">unit:Kill(true, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0158}}<syntaxhighlight lang="lua">local iGoldReceived;</syntaxhighlight>
{{CodeLine5|0159}}<syntaxhighlight lang="lua">local iVPReceived;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0161}}<syntaxhighlight lang="lua">-- Grant gold and VP</syntaxhighlight>
{{CodeLine5|0162}}<syntaxhighlight lang="lua">if (iTotalCircumnavigators == 0) then</syntaxhighlight>
{{CodeLine5|0163}}<syntaxhighlight lang="lua">iGoldReceived = 200;</syntaxhighlight>
{{CodeLine5|0164}}<syntaxhighlight lang="lua">iVPReceived = 200;</syntaxhighlight>
{{CodeLine5|0165}}<syntaxhighlight lang="lua">elseif (iTotalCircumnavigators == 1) then</syntaxhighlight>
{{CodeLine5|0166}}<syntaxhighlight lang="lua">iGoldReceived = 100;</syntaxhighlight>
{{CodeLine5|0167}}<syntaxhighlight lang="lua">iVPReceived = 100;</syntaxhighlight>
{{CodeLine5|0168}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0169}}<syntaxhighlight lang="lua">iGoldReceived = 50;</syntaxhighlight>
{{CodeLine5|0170}}<syntaxhighlight lang="lua">iVPReceived = 50;</syntaxhighlight>
{{CodeLine5|0171}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0173}}<syntaxhighlight lang="lua">player:ChangeGold(iGoldReceived);</syntaxhighlight>
{{CodeLine5|0174}}<syntaxhighlight lang="lua">local iNumWondersToCredit = iVPReceived / GameDefines["SCORE_WONDER_MULTIPLIER"];</syntaxhighlight>
{{CodeLine5|0175}}<syntaxhighlight lang="lua">player:ChangeNumWorldWonders( iNumWondersToCredit );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0177}}<syntaxhighlight lang="lua">-- Put up dialog box</syntaxhighlight>
{{CodeLine5|0178}}<syntaxhighlight lang="lua">local popupInfo = {</syntaxhighlight>
{{CodeLine5|0179}}<syntaxhighlight lang="lua">Data1 = 500,</syntaxhighlight>
{{CodeLine5|0180}}<syntaxhighlight lang="lua">Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0181}}<syntaxhighlight lang="lua">}</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0183}}<syntaxhighlight lang="lua">-- Human player?</syntaxhighlight>
{{CodeLine5|0184}}<syntaxhighlight lang="lua">if (iPlayer == 0) then</syntaxhighlight>
{{CodeLine5|0185}}<syntaxhighlight lang="lua">if (iTotalCircumnavigators == 0) then</syntaxhighlight>
{{CodeLine5|0186}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_NEWWORLD_SCENARIO_FIRST_CIRCUMNAVIGATION", unit:GetName(), iGoldReceived, iVPReceived);</syntaxhighlight>
{{CodeLine5|0187}}<syntaxhighlight lang="lua">elseif (iTotalCircumnavigators == 1) then</syntaxhighlight>
{{CodeLine5|0188}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_NEWWORLD_SCENARIO_SECOND_CIRCUMNAVIGATION", unit:GetName(), iGoldReceived, iVPReceived);</syntaxhighlight>
{{CodeLine5|0189}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0190}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_NEWWORLD_SCENARIO_THIRD_CIRCUMNAVIGATION", unit:GetName(), iGoldReceived, iVPReceived);</syntaxhighlight>
{{CodeLine5|0191}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0192}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0193}}<syntaxhighlight lang="lua">local iRemaining = 2 - iTotalCircumnavigators;</syntaxhighlight>
{{CodeLine5|0194}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_NEWWORLD_SCENARIO_OTHER_CIRCUMNAVIGATION", player:GetName(), iRemaining);</syntaxhighlight>
{{CodeLine5|0195}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0197}}<syntaxhighlight lang="lua">UI.AddPopup(popupInfo);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0199}}<syntaxhighlight lang="lua">Game:ChangeNukesExploded(1);</syntaxhighlight>
{{CodeLine5|0200}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0201}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0202}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">-- Treasure unit that has reached capital?</syntaxhighlight>
{{CodeLine5|0205}}<syntaxhighlight lang="lua">if (unit:GetUnitType() == GameInfoTypes["UNIT_TREASURE"]) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0207}}<syntaxhighlight lang="lua">-- At my capital?</syntaxhighlight>
{{CodeLine5|0208}}<syntaxhighlight lang="lua">local capital = player:GetCapitalCity();</syntaxhighlight>
{{CodeLine5|0209}}<syntaxhighlight lang="lua">if (capital ~= nil and capital:GetX() == iX and capital:GetY() == iY) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0211}}<syntaxhighlight lang="lua">unit:Kill(true, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">-- Grant gold and VP</syntaxhighlight>
{{CodeLine5|0214}}<syntaxhighlight lang="lua">local iGoldReceived = 100;</syntaxhighlight>
{{CodeLine5|0215}}<syntaxhighlight lang="lua">local iVPReceived = 50;</syntaxhighlight>
{{CodeLine5|0216}}<syntaxhighlight lang="lua">player:ChangeGold(iGoldReceived);</syntaxhighlight>
{{CodeLine5|0217}}<syntaxhighlight lang="lua">player:ChangeScoreFromFutureTech(iVPReceived);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0219}}<syntaxhighlight lang="lua">-- Put out notification</syntaxhighlight>
{{CodeLine5|0220}}<syntaxhighlight lang="lua">local text;</syntaxhighlight>
{{CodeLine5|0221}}<syntaxhighlight lang="lua">local heading;</syntaxhighlight>
{{CodeLine5|0222}}<syntaxhighlight lang="lua">text = Locale.ConvertTextKey("TXT_KEY_NEWWORLD_SCENARIO_TREASURE_RETURNED", capital:GetName(), iGoldReceived, iVPReceived);</syntaxhighlight>
{{CodeLine5|0223}}<syntaxhighlight lang="lua">heading = Locale.ConvertTextKey("TXT_KEY_NEWWORLD_SCENARIO_TREASURE_RETURNED_SHORT");</syntaxhighlight>
{{CodeLine5|0224}}<syntaxhighlight lang="lua">player:AddNotification(NotificationTypes.NOTIFICATION_GENERIC, text, heading);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0226}}<syntaxhighlight lang="lua">if(iPlayer == Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeLine5|0227}}<syntaxhighlight lang="lua">if(capital:GetX() > 50) then</syntaxhighlight>
{{CodeLine5|0228}}<syntaxhighlight lang="lua">UI.UnlockAchievement("ACHIEVEMENT_SCENARIO_02_RETURN_TREASURE");</syntaxhighlight>
{{CodeLine5|0229}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0230}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0231}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0232}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0234}}<syntaxhighlight lang="lua">return true;</syntaxhighlight>
{{CodeLine5|0235}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1030}}<syntaxhighlight lang="lua">GameEvents.UnitSetXY.Add(UpdatePromotion);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0594}}<syntaxhighlight lang="lua">GameEvents.UnitSetXY.Add(function(iPlayer, iUnitID, iX, iY)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0596}}<syntaxhighlight lang="lua">local plot = Map.GetPlot(iX, iY);</syntaxhighlight>
{{CodeLine5|0597}}<syntaxhighlight lang="lua">local player = Players[iPlayer];</syntaxhighlight>
{{CodeLine5|0598}}<syntaxhighlight lang="lua">local unit = player:GetUnitByID(iUnitID);</syntaxhighlight>
{{CodeLine5|0599}}<syntaxhighlight lang="lua">if (unit == nil or unit:IsDelayedDeath()) then</syntaxhighlight>
{{CodeLine5|0600}}<syntaxhighlight lang="lua">return false;</syntaxhighlight>
{{CodeLine5|0601}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0602}}<syntaxhighlight lang="lua">local iNumCaravels = GetPersistentProperty("NumCaravels");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0604}}<syntaxhighlight lang="lua">-- Caravel that has reached China?</syntaxhighlight>
{{CodeLine5|0605}}<syntaxhighlight lang="lua">if (unit:GetUnitType() == GameInfoTypes["UNIT_CARAVEL"] and iNumCaravels < 5) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0607}}<syntaxhighlight lang="lua">-- Adjacent to plot owned by China?</syntaxhighlight>
{{CodeLine5|0608}}<syntaxhighlight lang="lua">local bAdjacentChina = IsAdjacentToChina (iX, iY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0610}}<syntaxhighlight lang="lua">if (bAdjacentChina and not player:IsMinorCiv() and not player:IsBarbarian()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0612}}<syntaxhighlight lang="lua">-- How many have already been?</syntaxhighlight>
{{CodeLine5|0613}}<syntaxhighlight lang="lua">iNumCaravels = iNumCaravels + 1;</syntaxhighlight>
{{CodeLine5|0614}}<syntaxhighlight lang="lua">SetPersistentProperty("NumCaravels", iNumCaravels);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0616}}<syntaxhighlight lang="lua">unit:Kill(true, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0618}}<syntaxhighlight lang="lua">local iVPReceived;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0620}}<syntaxhighlight lang="lua">-- Grant VP</syntaxhighlight>
{{CodeLine5|0621}}<syntaxhighlight lang="lua">iVPReceived = 600 - (iNumCaravels * 100);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0623}}<syntaxhighlight lang="lua">player:ChangeScoreFromFutureTech(iVPReceived);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0625}}<syntaxhighlight lang="lua">-- Put up dialog box</syntaxhighlight>
{{CodeLine5|0626}}<syntaxhighlight lang="lua">local popupInfo = {</syntaxhighlight>
{{CodeLine5|0627}}<syntaxhighlight lang="lua">Data1 = 500,</syntaxhighlight>
{{CodeLine5|0628}}<syntaxhighlight lang="lua">Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0629}}<syntaxhighlight lang="lua">}</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0631}}<syntaxhighlight lang="lua">-- Human player?</syntaxhighlight>
{{CodeLine5|0632}}<syntaxhighlight lang="lua">if (iPlayer == 0) then</syntaxhighlight>
{{CodeLine5|0633}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_CARAVEL", unit:GetName(), iVPReceived, (5 - iNumCaravels));</syntaxhighlight>
{{CodeLine5|0634}}<syntaxhighlight lang="lua">UI.AddPopup(popupInfo);</syntaxhighlight>
{{CodeLine5|0635}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0636}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_OTHER_CARAVEL", player:GetName(), iVPReceived, (5 - iNumCaravels));</syntaxhighlight>
{{CodeLine5|0637}}<syntaxhighlight lang="lua">UI.AddPopup(popupInfo);</syntaxhighlight>
{{CodeLine5|0638}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0639}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0640}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0642}}<syntaxhighlight lang="lua">-- Conquistador that has reached China?</syntaxhighlight>
{{CodeLine5|0643}}<syntaxhighlight lang="lua">if (unit:GetUnitType() == GameInfoTypes["UNIT_SPANISH_CONQUISTADOR"]) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0645}}<syntaxhighlight lang="lua">-- Adjacent to plot owned by China?</syntaxhighlight>
{{CodeLine5|0646}}<syntaxhighlight lang="lua">local bAdjacentChina = IsAdjacentToChina (iX, iY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0648}}<syntaxhighlight lang="lua">-- How many have already been?</syntaxhighlight>
{{CodeLine5|0649}}<syntaxhighlight lang="lua">local iNumConquistadors = GetPersistentProperty("NumConquistadors");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0651}}<syntaxhighlight lang="lua">if (bAdjacentChina and not player:IsMinorCiv() and not player:IsBarbarian() and iNumConquistadors < 3) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0653}}<syntaxhighlight lang="lua">local pTeam;</syntaxhighlight>
{{CodeLine5|0654}}<syntaxhighlight lang="lua">pTeam = Teams[player:GetTeam()];</syntaxhighlight>
{{CodeLine5|0655}}<syntaxhighlight lang="lua">if (pTeam:IsHasTech(GameInfoTypes["TECH_EXPLORATION"])) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0657}}<syntaxhighlight lang="lua">iNumConquistadors = iNumConquistadors + 1;</syntaxhighlight>
{{CodeLine5|0658}}<syntaxhighlight lang="lua">SetPersistentProperty("NumConquistadors", iNumConquistadors);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0660}}<syntaxhighlight lang="lua">unit:Kill(true, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0662}}<syntaxhighlight lang="lua">local iGoldReceived;</syntaxhighlight>
{{CodeLine5|0663}}<syntaxhighlight lang="lua">local iVPReceived;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0665}}<syntaxhighlight lang="lua">-- Grant gold and VP</syntaxhighlight>
{{CodeLine5|0666}}<syntaxhighlight lang="lua">iGoldReceived = 500;</syntaxhighlight>
{{CodeLine5|0667}}<syntaxhighlight lang="lua">iVPReceived = 250;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0669}}<syntaxhighlight lang="lua">player:ChangeGold(iGoldReceived);</syntaxhighlight>
{{CodeLine5|0670}}<syntaxhighlight lang="lua">player:ChangeScoreFromFutureTech(iVPReceived);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0672}}<syntaxhighlight lang="lua">-- Put up dialog box</syntaxhighlight>
{{CodeLine5|0673}}<syntaxhighlight lang="lua">local popupInfo = {</syntaxhighlight>
{{CodeLine5|0674}}<syntaxhighlight lang="lua">Data1 = 500,</syntaxhighlight>
{{CodeLine5|0675}}<syntaxhighlight lang="lua">Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0676}}<syntaxhighlight lang="lua">}</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0678}}<syntaxhighlight lang="lua">-- Human player?</syntaxhighlight>
{{CodeLine5|0679}}<syntaxhighlight lang="lua">if (iPlayer == 0) then</syntaxhighlight>
{{CodeLine5|0680}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_CONQUISTADOR", unit:GetName(), iGoldReceived, iVPReceived);</syntaxhighlight>
{{CodeLine5|0681}}<syntaxhighlight lang="lua">UI.AddPopup(popupInfo);</syntaxhighlight>
{{CodeLine5|0682}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0683}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0684}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0685}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0687}}<syntaxhighlight lang="lua">return true;</syntaxhighlight>
{{CodeLine5|0688}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitSetXY]]
[[Category:Civ5 Units API|UnitSetXY]]