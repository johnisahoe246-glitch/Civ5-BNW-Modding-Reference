{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNextPolicyCost<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0229}}<syntaxhighlight lang="lua">local szText = Locale.ConvertTextKey("TXT_KEY_NEXT_POLICY_COST_LABEL", player:GetNextPolicyCost());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0239}}<syntaxhighlight lang="lua">local iCultureNeeded = player:GetNextPolicyCost() - player:GetJONSCulture();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0284}}<syntaxhighlight lang="lua">if player:GetJONSCulture() >= player:GetNextPolicyCost() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0357}}<syntaxhighlight lang="lua">strToolTip = strToolTip .. " " .. Locale.ConvertTextKey("TXT_KEY_POLICY_BRANCH_CANNOT_UNLOCK_CULTURE", player:GetNextPolicyCost());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0367}}<syntaxhighlight lang="lua">strToolTip = strToolTip .. "[NEWLINE][NEWLINE]" .. Locale.ConvertTextKey("TXT_KEY_POLICY_BRANCH_UNLOCK_SPEND", player:GetNextPolicyCost());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0135}}<syntaxhighlight lang="lua">if (pPlayer:GetNextPolicyCost() > 0) then</syntaxhighlight>
{{CodeLine5|0136}}<syntaxhighlight lang="lua">strCultureStr = string.format("%i/%i (+%i)", pPlayer:GetJONSCulture(), pPlayer:GetNextPolicyCost(), pPlayer:GetTotalJONSCulturePerTurn());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0749}}<syntaxhighlight lang="lua">local iCultureNeeded = pPlayer:GetNextPolicyCost() - pPlayer:GetJONSCulture();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0769}}<syntaxhighlight lang="lua">strText = strText .. Locale.ConvertTextKey("TXT_KEY_TP_CULTURE_NEXT_POLICY", pPlayer:GetNextPolicyCost());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNextPolicyCost]]
[[Category:Civ5 Policies API|GetNextPolicyCost]]