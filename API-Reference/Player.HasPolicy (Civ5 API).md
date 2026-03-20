{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:HasPolicy<b>(</b>{{Type5|PolicyType}} policy<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|policy:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0088}}<syntaxhighlight lang="lua">if (pOtherPlayer:HasPolicy(iPolicy)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0870}}<syntaxhighlight lang="lua">if (pPlayer:HasPolicy(i) and (not pPlayer:IsPolicyBlocked(i))) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">local bHasPolicy = player:HasPolicy(policyIndex);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0456}}<syntaxhighlight lang="lua">if player:HasPolicy( i ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0064}}<syntaxhighlight lang="lua">if (pPlayer:HasPolicy(GameInfo.Policies["POLICY_BARBARIAN_FINISHER"].ID) or pPlayer:HasPolicy(GameInfo.Policies["POLICY_SASSANID_FINISHER"].ID)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0257}}<syntaxhighlight lang="lua">if (Players[iPlayer]:HasPolicy(GameInfo.Policies["POLICY_BARBARIAN_FINISHER"].ID)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0266}}<syntaxhighlight lang="lua">if (Players[iPlayer]:HasPolicy(GameInfo.Policies["POLICY_SASSANID_FINISHER"].ID)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|HasPolicy]]
[[Category:Civ5 Policies API|HasPolicy]]