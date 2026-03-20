{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsPolicyBlocked<b>(</b>{{Type5|PolicyType}} i<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|i:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0870}}<syntaxhighlight lang="lua">if (pPlayer:HasPolicy(i) and (not pPlayer:IsPolicyBlocked(i))) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">print("Policy Blocked: " .. tostring(player:IsPolicyBlocked(policyIndex)));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0090}}<syntaxhighlight lang="lua">if (player:IsPolicyBlocked(policyIndex)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0505}}<syntaxhighlight lang="lua">if player:IsPolicyBlocked(i) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsPolicyBlocked]]
[[Category:Civ5 Policies API|IsPolicyBlocked]]