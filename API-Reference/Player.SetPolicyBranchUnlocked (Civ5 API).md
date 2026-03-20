{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Player:SetPolicyBranchUnlocked<b>(</b>{{Type5|PolicyBranchType}} arg0, '''bool''' arg1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0987}}<syntaxhighlight lang="lua">pPlayer:SetPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_ROMAN"].ID, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0990}}<syntaxhighlight lang="lua">pPlayer:SetPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_SASSANID"].ID, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0993}}<syntaxhighlight lang="lua">pPlayer:SetPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_BARBARIAN"].ID, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0821}}<syntaxhighlight lang="lua">pPlayer:SetPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_LABOR"].ID, true);</syntaxhighlight>
{{CodeLine5|0822}}<syntaxhighlight lang="lua">pPlayer:SetPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_CULTURE"].ID, true);</syntaxhighlight>
{{CodeLine5|0823}}<syntaxhighlight lang="lua">pPlayer:SetPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_INDUSTRY"].ID, true);</syntaxhighlight>
{{CodeLine5|0824}}<syntaxhighlight lang="lua">pPlayer:SetPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_COMMERCE"].ID, true);</syntaxhighlight>
{{CodeLine5|0825}}<syntaxhighlight lang="lua">pPlayer:SetPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_MILITARY"].ID, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetPolicyBranchUnlocked]]
[[Category:Civ5 Policies API|SetPolicyBranchUnlocked]]