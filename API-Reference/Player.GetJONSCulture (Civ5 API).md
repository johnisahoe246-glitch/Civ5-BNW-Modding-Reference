{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetJONSCulture<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0232}}<syntaxhighlight lang="lua">szText = Locale.ConvertTextKey("TXT_KEY_CURRENT_CULTURE_LABEL", player:GetJONSCulture());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0239}}<syntaxhighlight lang="lua">local iCultureNeeded = player:GetNextPolicyCost() - player:GetJONSCulture();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0284}}<syntaxhighlight lang="lua">if player:GetJONSCulture() >= player:GetNextPolicyCost() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">strCultureStr = string.format("%i/%i (+%i)", pPlayer:GetJONSCulture(), pPlayer:GetNextPolicyCost(), pPlayer:GetTotalJONSCulturePerTurn());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0138}}<syntaxhighlight lang="lua">strCultureStr = string.format("%i (+%i)", pPlayer:GetJONSCulture(), pPlayer:GetTotalJONSCulturePerTurn());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0749}}<syntaxhighlight lang="lua">local iCultureNeeded = pPlayer:GetNextPolicyCost() - pPlayer:GetJONSCulture();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0765}}<syntaxhighlight lang="lua">strText = strText .. Locale.ConvertTextKey("TXT_KEY_TP_CULTURE_ACCUMULATED", pPlayer:GetJONSCulture());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0065}}<syntaxhighlight lang="lua">if (pPlayer:GetTotalJONSCulturePerTurn() + pPlayer:GetJONSCulture() > 0) then</syntaxhighlight>
{{CodeLine5|0066}}<syntaxhighlight lang="lua">iGoldPerTurn = iGoldPerTurn + math.floor((pPlayer:GetTotalJONSCulturePerTurn() + pPlayer:GetJONSCulture()) / 3);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0475}}<syntaxhighlight lang="lua">iGoldPerTurnFromCulture = math.floor((pPlayer:GetTotalJONSCulturePerTurn() + pPlayer:GetJONSCulture()) / 3);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0258}}<syntaxhighlight lang="lua">if (Players[iPlayer]:GetJONSCulture() > 0) then</syntaxhighlight>
{{CodeLine5|0259}}<syntaxhighlight lang="lua">local iDiv = Players[iPlayer]:GetJONSCulture() / 3;</syntaxhighlight>
{{CodeLine5|0260}}<syntaxhighlight lang="lua">local iMod = Players[iPlayer]:GetJONSCulture() % 3;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetJONSCulture]]
[[Category:Civ5 Culture API|GetJONSCulture]]