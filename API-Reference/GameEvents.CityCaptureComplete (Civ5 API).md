{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


This event is triggered when a city is captured. We may infer from the name that it is triggered when the capture has been completed, the city now shows as owned by the conqueror, and buildings have been destroyed (''this has not been confirmed''). We might hope that there is a matching event when the capture has been determined, but ownership not yet changed and buildings not yet destroyed, but have no information on this as yet.


=Usage=
<code>'''void''' GameEvents.CityCaptureComplete<b>(</b>{{Type5|PlayerID}} player, '''int''' capital, {{Type5|ResourceType}} x, {{Type5|ResourceType}} y, {{Type5|PlayerID}} newPlayer, '''int''' conquest, '''int''' conquest<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''Presumably the player who lost the city''
|-
|valign="top" style="padding-right:6px;"|capital:
|valign="top"| ''Presumably true if the city captured is a capital''
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''Location of the city''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newPlayer:
|valign="top"| ''Presumably the player who captured the city''
|-
|valign="top" style="padding-right:6px;"|conquest:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|conquest:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 3 are listed.''

{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0500}}<syntaxhighlight lang="lua">GameEvents.CityCaptureComplete.Add(OnCityCaptured);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0185}}<syntaxhighlight lang="lua">GameEvents.CityCaptureComplete.Add(function(iOldOwner, bIsCapital, iX, iY, iNewOwner, iPop, bConquest)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0187}}<syntaxhighlight lang="lua">local plot = Map.GetPlot(iX, iY);</syntaxhighlight>
{{CodeLine5|0188}}<syntaxhighlight lang="lua">local cCity = plot:GetPlotCity();</syntaxhighlight>
{{CodeLine5|0189}}<syntaxhighlight lang="lua">local iNewOwner = cCity:GetOwner();</syntaxhighlight>
{{CodeLine5|0190}}<syntaxhighlight lang="lua">local civType = Players[iNewOwner]:GetCivilizationType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0192}}<syntaxhighlight lang="lua">local pOrthodoxHolyCity = Game.GetHolyCityForReligion(GameInfoTypes["RELIGION_ORTHODOXY"], -1);</syntaxhighlight>
{{CodeLine5|0193}}<syntaxhighlight lang="lua">local pIslamHolyCity = Game.GetHolyCityForReligion(GameInfoTypes["RELIGION_ISLAM"], -1);</syntaxhighlight>
{{CodeLine5|0194}}<syntaxhighlight lang="lua">local pChristianityHolyCity = Game.GetHolyCityForReligion(GameInfoTypes["RELIGION_CHRISTIANITY"], -1);</syntaxhighlight>
{{CodeLine5|0195}}<syntaxhighlight lang="lua">local pProtestantHolyCity = Game.GetHolyCityForReligion(GameInfoTypes["RELIGION_PROTESTANTISM"], -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0197}}<syntaxhighlight lang="lua">local popupInfo = {</syntaxhighlight>
{{CodeLine5|0198}}<syntaxhighlight lang="lua">Data1 = 500,</syntaxhighlight>
{{CodeLine5|0199}}<syntaxhighlight lang="lua">Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0200}}<syntaxhighlight lang="lua">}</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0202}}<syntaxhighlight lang="lua">if (cCity == pOrthodoxHolyCity) then</syntaxhighlight>
{{CodeLine5|0203}}<syntaxhighlight lang="lua">if (civType == GameInfo.Civilizations["CIVILIZATION_BYZANTIUM"].ID or</syntaxhighlight>
{{CodeLine5|0204}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_RUSSIA"].ID) then</syntaxhighlight>
{{CodeLine5|0205}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ORTHODOXY"], iNewOwner);</syntaxhighlight>
{{CodeLine5|0206}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0207}}<syntaxhighlight lang="lua">local pNewHolyCity = FindNextOrthodoxHolyCity();</syntaxhighlight>
{{CodeLine5|0208}}<syntaxhighlight lang="lua">if (pNewHolyCity == nil) then</syntaxhighlight>
{{CodeLine5|0209}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_NO_ORTHODOX_CITIES", pOrthodoxHolyCity:GetName(), pOrthodoxHolyCity:GetName());</syntaxhighlight>
{{CodeLine5|0210}}<syntaxhighlight lang="lua">UI.AddPopup(popupInfo);</syntaxhighlight>
{{CodeLine5|0211}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0212}}<syntaxhighlight lang="lua">Game.SetHolyCity (GameInfoTypes["RELIGION_ORTHODOXY"], pNewHolyCity);</syntaxhighlight>
{{CodeLine5|0213}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ORTHODOXY"], pNewHolyCity:GetOwner());</syntaxhighlight>
{{CodeLine5|0214}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_NEW_ORTHODOX_HOLY_CITY", pOrthodoxHolyCity:GetName(), pNewHolyCity:GetName());</syntaxhighlight>
{{CodeLine5|0215}}<syntaxhighlight lang="lua">UI.AddPopup(popupInfo);</syntaxhighlight>
{{CodeLine5|0216}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0217}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0219}}<syntaxhighlight lang="lua">elseif (cCity == pIslamHolyCity) then</syntaxhighlight>
{{CodeLine5|0220}}<syntaxhighlight lang="lua">if (civType == GameInfo.Civilizations["CIVILIZATION_SONGHAI"].ID or</syntaxhighlight>
{{CodeLine5|0221}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_OTTOMAN"].ID or</syntaxhighlight>
{{CodeLine5|0222}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_ARABIA"].ID) then</syntaxhighlight>
{{CodeLine5|0223}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ISLAM"], iNewOwner);</syntaxhighlight>
{{CodeLine5|0224}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0225}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ISLAM"], GetPersistentProperty("MeccaPlayer"));</syntaxhighlight>
{{CodeLine5|0226}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0228}}<syntaxhighlight lang="lua">elseif (cCity == pChristianityHolyCity) then</syntaxhighlight>
{{CodeLine5|0229}}<syntaxhighlight lang="lua">if (MyCurrentReligion(iNewOwner) == 2 and</syntaxhighlight>
{{CodeLine5|0230}}<syntaxhighlight lang="lua">(civType == GameInfo.Civilizations["CIVILIZATION_FRANCE"].ID or</syntaxhighlight>
{{CodeLine5|0231}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_CELTS"].ID or</syntaxhighlight>
{{CodeLine5|0232}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_ENGLAND"].ID or</syntaxhighlight>
{{CodeLine5|0233}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_SPAIN"].ID or</syntaxhighlight>
{{CodeLine5|0234}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_NETHERLANDS"].ID or</syntaxhighlight>
{{CodeLine5|0235}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_AUSTRIA"].ID or</syntaxhighlight>
{{CodeLine5|0236}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_SWEDEN"].ID)) then</syntaxhighlight>
{{CodeLine5|0237}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_CHRISTIANITY"], iNewOwner);</syntaxhighlight>
{{CodeLine5|0238}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0239}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_CHRISTIANITY"], GetPersistentProperty("VaticanPlayer"));</syntaxhighlight>
{{CodeLine5|0240}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0242}}<syntaxhighlight lang="lua">elseif (cCity == pProtestantHolyCity) then</syntaxhighlight>
{{CodeLine5|0243}}<syntaxhighlight lang="lua">if (MyCurrentReligion(iNewOwner) == 13 and</syntaxhighlight>
{{CodeLine5|0244}}<syntaxhighlight lang="lua">(civType == GameInfo.Civilizations["CIVILIZATION_FRANCE"].ID or</syntaxhighlight>
{{CodeLine5|0245}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_CELTS"].ID or</syntaxhighlight>
{{CodeLine5|0246}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_ENGLAND"].ID or</syntaxhighlight>
{{CodeLine5|0247}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_SPAIN"].ID or</syntaxhighlight>
{{CodeLine5|0248}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_NETHERLANDS"].ID or</syntaxhighlight>
{{CodeLine5|0249}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_AUSTRIA"].ID or</syntaxhighlight>
{{CodeLine5|0250}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_SWEDEN"].ID)) then</syntaxhighlight>
{{CodeLine5|0251}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_PROTESTANTISM"], iNewOwner);</syntaxhighlight>
{{CodeLine5|0252}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0253}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_PROTESTANTISM"], GetPersistentProperty("ProtestantHolyCityPlayer"));</syntaxhighlight>
{{CodeLine5|0254}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0256}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0258}}<syntaxhighlight lang="lua">-- VP for capture?</syntaxhighlight>
{{CodeLine5|0259}}<syntaxhighlight lang="lua">local eCityReligion = cCity:GetReligiousMajority();</syntaxhighlight>
{{CodeLine5|0260}}<syntaxhighlight lang="lua">local eCapturingPlayerReligion = MyCurrentReligion(iNewOwner);</syntaxhighlight>
{{CodeLine5|0261}}<syntaxhighlight lang="lua">local player = Players[iNewOwner];</syntaxhighlight>
{{CodeLine5|0262}}<syntaxhighlight lang="lua">local pJerusalemPlot = Map.GetPlot(GetPersistentProperty("JerusalemX"), GetPersistentProperty("JerusalemY"));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0264}}<syntaxhighlight lang="lua">if (bConquest and eCityReligion ~= eCapturingPlayerReligion and eCityReligion > 0 and iNewOwner < 22) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0266}}<syntaxhighlight lang="lua">local iVPReceived = iPop * 25;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0268}}<syntaxhighlight lang="lua">-- Put up dialog box</syntaxhighlight>
{{CodeLine5|0269}}<syntaxhighlight lang="lua">local popupInfo = {</syntaxhighlight>
{{CodeLine5|0270}}<syntaxhighlight lang="lua">Data1 = 500,</syntaxhighlight>
{{CodeLine5|0271}}<syntaxhighlight lang="lua">Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0272}}<syntaxhighlight lang="lua">}</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">-- Human player?</syntaxhighlight>
{{CodeLine5|0275}}<syntaxhighlight lang="lua">if (cCity:IsHolyCityAnyReligion() or cCity:Plot() == pJerusalemPlot) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0277}}<syntaxhighlight lang="lua">iVPReceived = iVPReceived * 2;</syntaxhighlight>
{{CodeLine5|0278}}<syntaxhighlight lang="lua">player:ChangeScoreFromFutureTech(iVPReceived);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0280}}<syntaxhighlight lang="lua">if (iPlayer == 0) then</syntaxhighlight>
{{CodeLine5|0281}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_VP_HOLY_CITY_CAPTURE_HUMAN", iVPReceived, cCity:GetName(), iPop);</syntaxhighlight>
{{CodeLine5|0282}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0283}}<syntaxhighlight lang="lua">if (Teams[player:GetTeam()]:IsHasMet(Game.GetActiveTeam())) then</syntaxhighlight>
{{CodeLine5|0284}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_VP_HOLY_CITY_CAPTURE", player:GetCivilizationDescriptionKey(), iVPReceived, cCity:GetName(), iPop);</syntaxhighlight>
{{CodeLine5|0285}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0286}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_VP_HOLY_CITY_CAPTURE", "TXT_KEY_UNMET_PLAYER", iVPReceived, cCity:GetName(), iPop);</syntaxhighlight>
{{CodeLine5|0287}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0288}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0289}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0291}}<syntaxhighlight lang="lua">player:ChangeScoreFromFutureTech(iVPReceived);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0293}}<syntaxhighlight lang="lua">if (iPlayer == 0) then</syntaxhighlight>
{{CodeLine5|0294}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_VP_CITY_CAPTURE_HUMAN", iVPReceived, cCity:GetName(), iPop);</syntaxhighlight>
{{CodeLine5|0295}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0296}}<syntaxhighlight lang="lua">if (Teams[player:GetTeam()]:IsHasMet(Game.GetActiveTeam())) then</syntaxhighlight>
{{CodeLine5|0297}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_VP_CITY_CAPTURE", player:GetCivilizationDescriptionKey(), iVPReceived, cCity:GetName(), iPop);</syntaxhighlight>
{{CodeLine5|0298}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0299}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_VP_CITY_CAPTURE", "TXT_KEY_UNMET_PLAYER", iVPReceived, cCity:GetName(), iPop);</syntaxhighlight>
{{CodeLine5|0300}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0301}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0302}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0303}}<syntaxhighlight lang="lua">UI.AddPopup(popupInfo);</syntaxhighlight>
{{CodeLine5|0304}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0305}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CityCaptureComplete]]
[[Category:Civ5 Cities API|CityCaptureComplete]]
[[Category:Civ5 Combat API|CityCaptureComplete]]