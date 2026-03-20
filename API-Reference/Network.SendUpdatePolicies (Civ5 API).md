{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendUpdatePolicies<b>(</b>'''int''' newPolicyBranch, '''bool''' policy, '''bool''' arg2<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|newPolicyBranch:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|policy:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ConfirmPolicyBranchPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ConfirmPolicyBranchPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0035}}<syntaxhighlight lang="lua">Network.SendUpdatePolicies(iNewPolicyBranch, bPolicy, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0904}}<syntaxhighlight lang="lua">Network.SendUpdatePolicies(m_gPolicyID, m_gAdoptingPolicy, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendUpdatePolicies]]
[[Category:Civ5 Policies API|SendUpdatePolicies]]