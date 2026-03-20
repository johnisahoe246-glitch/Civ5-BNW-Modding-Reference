{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:CanUnlockPolicyBranch<b>(</b>'''int''' policyBranch<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|policyBranch:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">local bCanAdoptPolicyBranch = player:CanUnlockPolicyBranch(policyBranchIndex);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0337}}<syntaxhighlight lang="lua">if (not player:CanUnlockPolicyBranch(i)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanUnlockPolicyBranch]]
[[Category:Civ5 Policies API|CanUnlockPolicyBranch]]