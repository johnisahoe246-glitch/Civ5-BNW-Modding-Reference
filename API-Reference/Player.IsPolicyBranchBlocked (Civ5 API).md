{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsPolicyBranchBlocked<b>(</b>{{Type5|PolicyBranchType}} policyBranchIndex<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|policyBranchIndex:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0269}}<syntaxhighlight lang="lua">return (policy ~= nil and player:IsPolicyBranchUnlocked(policy.ID) and not player:IsPolicyBranchBlocked(policy.ID));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0148}}<syntaxhighlight lang="lua">if (player:IsPolicyBranchBlocked(policyBranchIndex)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0386}}<syntaxhighlight lang="lua">elseif (player:IsPolicyBranchBlocked(i)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0972}}<syntaxhighlight lang="lua">if (info.ID == GameInfo.Units["UNIT_MERCHANT"].ID and pPlayer:IsPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_COMMERCE"].ID) and not pPlayer:IsPolicyBranchBlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_COMMERCE"].ID)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0977}}<syntaxhighlight lang="lua">if (info.ID == GameInfo.Units["UNIT_SCIENTIST"].ID and pPlayer:IsPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_RATIONALISM"].ID) and not pPlayer:IsPolicyBranchBlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_RATIONALISM"].ID)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0982}}<syntaxhighlight lang="lua">if (info.ID == GameInfo.Units["UNIT_ARTIST"].ID and pPlayer:IsPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_FREEDOM"].ID) and not pPlayer:IsPolicyBranchBlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_FREEDOM"].ID)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0987}}<syntaxhighlight lang="lua">if (info.ID == GameInfo.Units["UNIT_GREAT_GENERAL"].ID and pPlayer:IsPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_AUTOCRACY"].ID) and not pPlayer:IsPolicyBranchBlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_AUTOCRACY"].ID)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0992}}<syntaxhighlight lang="lua">if (info.ID == GameInfo.Units["UNIT_GREAT_ADMIRAL"].ID and pPlayer:IsPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_AUTOCRACY"].ID) and not pPlayer:IsPolicyBranchBlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_AUTOCRACY"].ID)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0997}}<syntaxhighlight lang="lua">if (info.ID == GameInfo.Units["UNIT_ENGINEER"].ID and pPlayer:IsPolicyBranchUnlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_ORDER"].ID) and not pPlayer:IsPolicyBranchBlocked(GameInfo.PolicyBranchTypes["POLICY_BRANCH_ORDER"].ID)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsPolicyBranchBlocked]]
[[Category:Civ5 Policies API|IsPolicyBranchBlocked]]