{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNumPolicyBranchesFinished<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0523}}<syntaxhighlight lang="lua">local numDone = player:GetNumPolicyBranchesFinished();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0447}}<syntaxhighlight lang="lua">if(not v:IsMinorCiv() and v:IsAlive() and (leadAI == nil or v:GetNumPolicyBranchesFinished() > maxPolicies) and i ~= Game.GetActivePlayer()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0449}}<syntaxhighlight lang="lua">maxPolicies = v:GetNumPolicyBranchesFinished();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0469}}<syntaxhighlight lang="lua">Controls.CultureLabel:SetText(Locale.ConvertTextKey("TXT_KEY_VP_DIPLO_SOCIAL_POLICIES", strCiv, leadAI:GetNumPolicyBranchesFinished(), numBranchesRequiredForUtopia));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0774}}<syntaxhighlight lang="lua">table.sort(sortedPlayerList, function(a, b) return Players[b]:GetNumPolicyBranchesFinished() <</syntaxhighlight>
{{CodeLine5|0775}}<syntaxhighlight lang="lua">Players[a]:GetNumPolicyBranchesFinished() end );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0812}}<syntaxhighlight lang="lua">local numPoliciesFinished = pPlayer:GetNumPolicyBranchesFinished();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumPolicyBranchesFinished]]
[[Category:Civ5 Policies API|GetNumPolicyBranchesFinished]]