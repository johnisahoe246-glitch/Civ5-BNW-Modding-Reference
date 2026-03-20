{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNumCities<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1247}}<syntaxhighlight lang="lua">for cityIndex = 0, player:GetNumCities() - 1, 1</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0709}}<syntaxhighlight lang="lua">if (pPlayer:GetNumCities() <= 1) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">if (Players[playerID]:GetNumCities() == 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0190}}<syntaxhighlight lang="lua">local iExtraHappinessPerCity = pPlayer:GetExtraHappinessPerCity() * pPlayer:GetNumCities();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0405}}<syntaxhighlight lang="lua">local iNumNormalCities = pPlayer:GetNumCities() - iNumOccupiedCities;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0587}}<syntaxhighlight lang="lua">if( pPlayer:GetNumCities() > 0 ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0811}}<syntaxhighlight lang="lua">if (UI.CanSelectionListFound() and player:GetNumCities() > 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0223}}<syntaxhighlight lang="lua">local playerHas1City = player:GetNumCities() > 0;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0013}}<syntaxhighlight lang="lua">if (pPlayer:GetNumCities() > 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0315}}<syntaxhighlight lang="lua">for cityIndex = 0, pPlayer:GetNumCities() - 1, 1 do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1123}}<syntaxhighlight lang="lua">if (pPlayer:IsAlive() and pPlayer:GetNumCities() == 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0516}}<syntaxhighlight lang="lua">if (not pPlayer:IsMinorCiv() and pPlayer:GetNumCities() == 1) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0305}}<syntaxhighlight lang="lua">if (player:GetNumCities() > 1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0512}}<syntaxhighlight lang="lua">if (player:GetNumMilitaryUnits() <= player:GetNumCities()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0625}}<syntaxhighlight lang="lua">if (player:GetNumCities() == 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1304}}<syntaxhighlight lang="lua">if (player:GetNumCities() > 3) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1322}}<syntaxhighlight lang="lua">if (iNumWorkers > player:GetNumCities()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1596}}<syntaxhighlight lang="lua">if (player:GetNumCities() <= 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3316}}<syntaxhighlight lang="lua">if (player:GetNumCities() > 0) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumCities]]
[[Category:Civ5 Cities API|GetNumCities]]