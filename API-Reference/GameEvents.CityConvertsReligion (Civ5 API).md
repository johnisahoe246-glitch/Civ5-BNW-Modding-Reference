{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
<br/>
*This method was added in Gods & Kings.
}}


=Usage=
<code>'''void''' GameEvents.CityConvertsReligion<b>(</b>{{Type5|PlayerID}} owner, {{Type5|ReligionType}} religion, '''int''' x, '''int''' y<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|owner:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|religion:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 1 are listed.''

{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0711}}<syntaxhighlight lang="lua">GameEvents.CityConvertsReligion.Add(function(iOwner, eReligion, iX, iY)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0713}}<syntaxhighlight lang="lua">-- Only matters if switched to Protestant</syntaxhighlight>
{{CodeLine5|0714}}<syntaxhighlight lang="lua">if (eReligion == 13) then</syntaxhighlight>
{{CodeLine5|0715}}<syntaxhighlight lang="lua">local pPlayer = Players[iOwner];</syntaxhighlight>
{{CodeLine5|0716}}<syntaxhighlight lang="lua">local civType = pPlayer:GetCivilizationType();</syntaxhighlight>
{{CodeLine5|0717}}<syntaxhighlight lang="lua">if (civType == GameInfo.Civilizations["CIVILIZATION_FRANCE"].ID or</syntaxhighlight>
{{CodeLine5|0718}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_CELTS"].ID or</syntaxhighlight>
{{CodeLine5|0719}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_ENGLAND"].ID or</syntaxhighlight>
{{CodeLine5|0720}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_SPAIN"].ID or</syntaxhighlight>
{{CodeLine5|0721}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_NETHERLANDS"].ID or</syntaxhighlight>
{{CodeLine5|0722}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_AUSTRIA"].ID or</syntaxhighlight>
{{CodeLine5|0723}}<syntaxhighlight lang="lua">civType == GameInfo.Civilizations["CIVILIZATION_SWEDEN"].ID) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0725}}<syntaxhighlight lang="lua">if (pPlayer:HasReligionInMostCities(eReligion)) then</syntaxhighlight>
{{CodeLine5|0726}}<syntaxhighlight lang="lua">local bChangeMade = false;</syntaxhighlight>
{{CodeLine5|0727}}<syntaxhighlight lang="lua">if (civType == GameInfo.Civilizations["CIVILIZATION_FRANCE"].ID) then</syntaxhighlight>
{{CodeLine5|0728}}<syntaxhighlight lang="lua">if (GetPersistentProperty("FranceCatholic") == 1) then</syntaxhighlight>
{{CodeLine5|0729}}<syntaxhighlight lang="lua">SetPersistentProperty("FranceCatholic", 0);</syntaxhighlight>
{{CodeLine5|0730}}<syntaxhighlight lang="lua">bChangeMade = true;</syntaxhighlight>
{{CodeLine5|0731}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0732}}<syntaxhighlight lang="lua">elseif (civType == GameInfo.Civilizations["CIVILIZATION_CELTS"].ID) then</syntaxhighlight>
{{CodeLine5|0733}}<syntaxhighlight lang="lua">if (GetPersistentProperty("CeltsCatholic") == 1) then</syntaxhighlight>
{{CodeLine5|0734}}<syntaxhighlight lang="lua">SetPersistentProperty("CeltsCatholic", 0);</syntaxhighlight>
{{CodeLine5|0735}}<syntaxhighlight lang="lua">bChangeMade = true;</syntaxhighlight>
{{CodeLine5|0736}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0737}}<syntaxhighlight lang="lua">elseif (civType == GameInfo.Civilizations["CIVILIZATION_ENGLAND"].ID) then</syntaxhighlight>
{{CodeLine5|0738}}<syntaxhighlight lang="lua">if (GetPersistentProperty("EnglandCatholic") == 1) then</syntaxhighlight>
{{CodeLine5|0739}}<syntaxhighlight lang="lua">SetPersistentProperty("EnglandCatholic", 0);</syntaxhighlight>
{{CodeLine5|0740}}<syntaxhighlight lang="lua">bChangeMade = true;</syntaxhighlight>
{{CodeLine5|0741}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0742}}<syntaxhighlight lang="lua">elseif (civType == GameInfo.Civilizations["CIVILIZATION_SPAIN"].ID) then</syntaxhighlight>
{{CodeLine5|0743}}<syntaxhighlight lang="lua">if (GetPersistentProperty("SpainCatholic") == 1) then</syntaxhighlight>
{{CodeLine5|0744}}<syntaxhighlight lang="lua">SetPersistentProperty("SpainCatholic", 0);</syntaxhighlight>
{{CodeLine5|0745}}<syntaxhighlight lang="lua">bChangeMade = true;</syntaxhighlight>
{{CodeLine5|0746}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0747}}<syntaxhighlight lang="lua">elseif (civType == GameInfo.Civilizations["CIVILIZATION_NETHERLANDS"].ID) then</syntaxhighlight>
{{CodeLine5|0748}}<syntaxhighlight lang="lua">if (GetPersistentProperty("NetherlandsCatholic") == 1) then</syntaxhighlight>
{{CodeLine5|0749}}<syntaxhighlight lang="lua">SetPersistentProperty("NetherlandsCatholic", 0);</syntaxhighlight>
{{CodeLine5|0750}}<syntaxhighlight lang="lua">bChangeMade = true;</syntaxhighlight>
{{CodeLine5|0751}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0752}}<syntaxhighlight lang="lua">elseif (civType == GameInfo.Civilizations["CIVILIZATION_AUSTRIA"].ID) then</syntaxhighlight>
{{CodeLine5|0753}}<syntaxhighlight lang="lua">if (GetPersistentProperty("AustriaCatholic") == 1) then</syntaxhighlight>
{{CodeLine5|0754}}<syntaxhighlight lang="lua">SetPersistentProperty("AustriaCatholic", 0);</syntaxhighlight>
{{CodeLine5|0755}}<syntaxhighlight lang="lua">bChangeMade = true;</syntaxhighlight>
{{CodeLine5|0756}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0757}}<syntaxhighlight lang="lua">elseif (civType == GameInfo.Civilizations["CIVILIZATION_SWEDEN"].ID) then</syntaxhighlight>
{{CodeLine5|0758}}<syntaxhighlight lang="lua">if (GetPersistentProperty("SwedenCatholic") == 1) then</syntaxhighlight>
{{CodeLine5|0759}}<syntaxhighlight lang="lua">SetPersistentProperty("SwedenCatholic", 0);</syntaxhighlight>
{{CodeLine5|0760}}<syntaxhighlight lang="lua">bChangeMade = true;</syntaxhighlight>
{{CodeLine5|0761}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0762}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0764}}<syntaxhighlight lang="lua">if (bChangeMade) then</syntaxhighlight>
{{CodeLine5|0765}}<syntaxhighlight lang="lua">local popupInfo = {</syntaxhighlight>
{{CodeLine5|0766}}<syntaxhighlight lang="lua">Data1 = 500,</syntaxhighlight>
{{CodeLine5|0767}}<syntaxhighlight lang="lua">Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0768}}<syntaxhighlight lang="lua">}</syntaxhighlight>
{{CodeLine5|0769}}<syntaxhighlight lang="lua">if (Game.GetActivePlayer() == iOwner) then</syntaxhighlight>
{{CodeLine5|0770}}<syntaxhighlight lang="lua">local pProtestantHolyCity = Game.GetHolyCityForReligion(GameInfoTypes["RELIGION_PROTESTANTISM"], -1);</syntaxhighlight>
{{CodeLine5|0771}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_YOU_ADOPTED_PROTESTANTISM", pProtestantHolyCity:GetName());</syntaxhighlight>
{{CodeLine5|0772}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0773}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_OTHER_ADOPTED_PROTESTANTISM", pPlayer:GetName());</syntaxhighlight>
{{CodeLine5|0774}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0775}}<syntaxhighlight lang="lua">UI.AddPopup(popupInfo);</syntaxhighlight>
{{CodeLine5|0776}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0777}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0778}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0779}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0780}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CityConvertsReligion]]
[[Category:Civ5 Cities API|CityConvertsReligion]]
[[Category:Civ5 Religion API|CityConvertsReligion]]