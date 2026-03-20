{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetTotalJONSCulturePerTurn<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0235}}<syntaxhighlight lang="lua">szText = Locale.ConvertTextKey("TXT_KEY_CULTURE_PER_TURN_LABEL", player:GetTotalJONSCulturePerTurn());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0243}}<syntaxhighlight lang="lua">if (player:GetTotalJONSCulturePerTurn() == 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0246}}<syntaxhighlight lang="lua">iTurns = iCultureNeeded / player:GetTotalJONSCulturePerTurn();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">strCultureStr = string.format("%i/%i (+%i)", pPlayer:GetJONSCulture(), pPlayer:GetNextPolicyCost(), pPlayer:GetTotalJONSCulturePerTurn());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0138}}<syntaxhighlight lang="lua">strCultureStr = string.format("%i (+%i)", pPlayer:GetJONSCulture(), pPlayer:GetTotalJONSCulturePerTurn());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0753}}<syntaxhighlight lang="lua">if (pPlayer:GetTotalJONSCulturePerTurn() == 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0756}}<syntaxhighlight lang="lua">iTurns = iCultureNeeded / pPlayer:GetTotalJONSCulturePerTurn();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0873}}<syntaxhighlight lang="lua">local iCultureFromGoldenAge = pPlayer:GetTotalJONSCulturePerTurn() - iCultureForFree - iCultureFromCities - iCultureFromHappiness - iCultureFromMinors - iCultureFromReligion;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0065}}<syntaxhighlight lang="lua">if (pPlayer:GetTotalJONSCulturePerTurn() + pPlayer:GetJONSCulture() > 0) then</syntaxhighlight>
{{CodeLine5|0066}}<syntaxhighlight lang="lua">iGoldPerTurn = iGoldPerTurn + math.floor((pPlayer:GetTotalJONSCulturePerTurn() + pPlayer:GetJONSCulture()) / 3);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0475}}<syntaxhighlight lang="lua">iGoldPerTurnFromCulture = math.floor((pPlayer:GetTotalJONSCulturePerTurn() + pPlayer:GetJONSCulture()) / 3);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTotalJONSCulturePerTurn]]
[[Category:Civ5 Culture API|GetTotalJONSCulturePerTurn]]
[[Category:Civ5 Score API|GetTotalJONSCulturePerTurn]]