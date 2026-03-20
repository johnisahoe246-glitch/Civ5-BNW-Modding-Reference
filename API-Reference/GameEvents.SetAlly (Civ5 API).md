{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


Triggered when the ally of a City-State changes (whether it changes from none or from another player).


=Usage=
<code>'''void''' GameEvents.SetAlly<b>(</b>{{Type5|PlayerID}} cSPlayer, {{Type5|PlayerID}} oldAlly, {{Type5|PlayerID}} newAlly<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|cSPlayer:
|valign="top"| ''The City-State player in question''
|-
|valign="top" style="padding-right:6px;"|oldAlly:
|valign="top"| ''The former ally of the City-State; presumably nil or similar if the CS did not have an ally''
|-
|valign="top" style="padding-right:6px;"|newAlly:
|valign="top"| ''The new ally of the City-State''
|}


=Source code samples=
''Too many occurences. Only 50 out of 2 are listed.''

{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0135}}<syntaxhighlight lang="lua">GameEvents.SetAlly.Add(function(iCSPlayer, iOldAlly, iNewAlly)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0137}}<syntaxhighlight lang="lua">print ("SetAlly called, params: " .. tostring(iCSPlayer) .. ", " .. tostring(iOldAlly) .. ", " .. tostring(iNewAlly));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0139}}<syntaxhighlight lang="lua">if (iNewAlly == -1) then</syntaxhighlight>
{{CodeLine5|0140}}<syntaxhighlight lang="lua">local pPlayer = Players[iOldAlly];</syntaxhighlight>
{{CodeLine5|0141}}<syntaxhighlight lang="lua">for unit in pPlayer:Units()</syntaxhighlight>
{{CodeLine5|0142}}<syntaxhighlight lang="lua">   do</syntaxhighlight>
{{CodeLine5|0143}}<syntaxhighlight lang="lua">   if (unit:IsCombatUnit() and unit:GetOriginalOwner() == iCSPlayer) then</syntaxhighlight>
{{CodeLine5|0144}}<syntaxhighlight lang="lua">   ChangeOwner(unit, iCSPlayer, -1);</syntaxhighlight>
{{CodeLine5|0145}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0146}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0147}}<syntaxhighlight lang="lua">   else</syntaxhighlight>
{{CodeLine5|0148}}<syntaxhighlight lang="lua">   local pPlayer = Players[iCSPlayer];</syntaxhighlight>
{{CodeLine5|0149}}<syntaxhighlight lang="lua">   for unit in pPlayer:Units()</syntaxhighlight>
{{CodeLine5|0150}}<syntaxhighlight lang="lua">   do</syntaxhighlight>
{{CodeLine5|0151}}<syntaxhighlight lang="lua">   if (unit:IsCombatUnit()) then</syntaxhighlight>
{{CodeLine5|0152}}<syntaxhighlight lang="lua">   ChangeOwner(unit, iNewAlly, iCSPlayer);</syntaxhighlight>
{{CodeLine5|0153}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0154}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0155}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0157}}<syntaxhighlight lang="lua">   if (iNewAlly == -1) then</syntaxhighlight>
{{CodeLine5|0158}}<syntaxhighlight lang="lua">   if (iOldAlly == Game.GetActivePlayer())   then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0160}}<syntaxhighlight lang="lua">   local strPlayerKey = Players[iCSPlayer]:GetCivilizationShortDescriptionKey();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0162}}<syntaxhighlight lang="lua">   -- Put up dialog box</syntaxhighlight>
{{CodeLine5|0163}}<syntaxhighlight lang="lua">   local popupInfo = {</syntaxhighlight>
{{CodeLine5|0164}}<syntaxhighlight lang="lua">   Data1 = 500,</syntaxhighlight>
{{CodeLine5|0165}}<syntaxhighlight lang="lua">   Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0166}}<syntaxhighlight lang="lua">   Text = Locale.ConvertTextKey("TXT_KEY_1066_SCENARIO_ALLY_LOST", strPlayerKey);</syntaxhighlight>
{{CodeLine5|0167}}<syntaxhighlight lang="lua">   }</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0169}}<syntaxhighlight lang="lua">   UI.AddPopup(popupInfo);</syntaxhighlight>
{{CodeLine5|0170}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0171}}<syntaxhighlight lang="lua">   else</syntaxhighlight>
{{CodeLine5|0172}}<syntaxhighlight lang="lua">   if (iNewAlly == Game.GetActivePlayer())   then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0174}}<syntaxhighlight lang="lua">   local strPlayerKey = Players[iCSPlayer]:GetCivilizationShortDescriptionKey();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0176}}<syntaxhighlight lang="lua">   -- Put up dialog box</syntaxhighlight>
{{CodeLine5|0177}}<syntaxhighlight lang="lua">   local popupInfo = {</syntaxhighlight>
{{CodeLine5|0178}}<syntaxhighlight lang="lua">   Data1 = 500,</syntaxhighlight>
{{CodeLine5|0179}}<syntaxhighlight lang="lua">   Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0180}}<syntaxhighlight lang="lua">   Text = Locale.ConvertTextKey("TXT_KEY_1066_SCENARIO_ALLY_GAINED", strPlayerKey);</syntaxhighlight>
{{CodeLine5|0181}}<syntaxhighlight lang="lua">   }</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0183}}<syntaxhighlight lang="lua">   UI.AddPopup(popupInfo);</syntaxhighlight>
{{CodeLine5|0184}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeLine5|0185}}<syntaxhighlight lang="lua">   end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0187}}<syntaxhighlight lang="lua">   end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0331}}<syntaxhighlight lang="lua">GameEvents.SetAlly.Add(function(iMinor, iOldAlly, iNewAlly)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0333}}<syntaxhighlight lang="lua">local iMeccaPlayer = GetPersistentProperty("MeccaPlayer");</syntaxhighlight>
{{CodeLine5|0334}}<syntaxhighlight lang="lua">local iVaticanPlayer = GetPersistentProperty("VaticanPlayer");</syntaxhighlight>
{{CodeLine5|0335}}<syntaxhighlight lang="lua">local iProtestantPlayer = GetPersistentProperty("ProtestantHolyCityPlayer")</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0337}}<syntaxhighlight lang="lua">if (iNewAlly == -1) then</syntaxhighlight>
{{CodeLine5|0338}}<syntaxhighlight lang="lua">if (iMinor == iMeccaPlayer) then</syntaxhighlight>
{{CodeLine5|0339}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ISLAM"], iMeccaPlayer);</syntaxhighlight>
{{CodeLine5|0340}}<syntaxhighlight lang="lua">elseif (iMinor == iVaticanPlayer) then</syntaxhighlight>
{{CodeLine5|0341}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_CHRISTIANITY"], iVaticanPlayer);</syntaxhighlight>
{{CodeLine5|0342}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0344}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0345}}<syntaxhighlight lang="lua">local civType = Players[iNewAlly]:GetCivilizationType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0347}}<syntaxhighlight lang="lua">if (iMinor == iMeccaPlayer) then</syntaxhighlight>
{{CodeLine5|0348}}<syntaxhighlight lang="lua">if (civType == GameInfo.Civilizations["CIVILIZATION_SONGHAI"].ID or</syntaxhighlight>
{{CodeLine5|0349}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_OTTOMAN"].ID or</syntaxhighlight>
{{CodeLine5|0350}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_ARABIA"].ID) then</syntaxhighlight>
{{CodeLine5|0351}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ISLAM"], iNewAlly);</syntaxhighlight>
{{CodeLine5|0352}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0353}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ISLAM"], iMeccaPlayer);</syntaxhighlight>
{{CodeLine5|0354}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0356}}<syntaxhighlight lang="lua">elseif (iMinor == iVaticanPlayer) then</syntaxhighlight>
{{CodeLine5|0357}}<syntaxhighlight lang="lua">if (MyCurrentReligion(iNewAlly) == 2 and</syntaxhighlight>
{{CodeLine5|0358}}<syntaxhighlight lang="lua">(civType == GameInfo.Civilizations["CIVILIZATION_FRANCE"].ID or</syntaxhighlight>
{{CodeLine5|0359}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_CELTS"].ID or</syntaxhighlight>
{{CodeLine5|0360}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_ENGLAND"].ID or</syntaxhighlight>
{{CodeLine5|0361}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_SPAIN"].ID or</syntaxhighlight>
{{CodeLine5|0362}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_NETHERLANDS"].ID or</syntaxhighlight>
{{CodeLine5|0363}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_AUSTRIA"].ID or</syntaxhighlight>
{{CodeLine5|0364}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_SWEDEN"].ID)) then</syntaxhighlight>
{{CodeLine5|0365}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_CHRISTIANITY"], iNewAlly);</syntaxhighlight>
{{CodeLine5|0366}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0367}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_CHRISTIANITY"], iVaticanPlayer);</syntaxhighlight>
{{CodeLine5|0368}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0370}}<syntaxhighlight lang="lua">elseif (iMinor == GetPersistentProperty("ProtestantHolyCityPlayer")) then</syntaxhighlight>
{{CodeLine5|0371}}<syntaxhighlight lang="lua">if (MyCurrentReligion(iNewAlly) == 13 and</syntaxhighlight>
{{CodeLine5|0372}}<syntaxhighlight lang="lua">(civType == GameInfo.Civilizations["CIVILIZATION_FRANCE"].ID or</syntaxhighlight>
{{CodeLine5|0373}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_CELTS"].ID or</syntaxhighlight>
{{CodeLine5|0374}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_ENGLAND"].ID or</syntaxhighlight>
{{CodeLine5|0375}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_SPAIN"].ID or</syntaxhighlight>
{{CodeLine5|0376}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_NETHERLANDS"].ID or</syntaxhighlight>
{{CodeLine5|0377}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_AUSTRIA"].ID or</syntaxhighlight>
{{CodeLine5|0378}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_SWEDEN"].ID)) then</syntaxhighlight>
{{CodeLine5|0379}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_PROTESTANTISM"], iNewAlly);</syntaxhighlight>
{{CodeLine5|0380}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0381}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_PROTESTANTISM"], iProtestantPlayer);</syntaxhighlight>
{{CodeLine5|0382}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0384}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0385}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0387}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetAlly]]
[[Category:Civ5 Diplomacy API|SetAlly]]