{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:CanAdoptPolicy<b>(</b>{{Type5|PolicyType}} policy<b>)</b></code>


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

{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0078}}<syntaxhighlight lang="lua">local bCanAdoptPolicy = player:CanAdoptPolicy(policyIndex);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0477}}<syntaxhighlight lang="lua">elseif player:CanAdoptPolicy( i ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanAdoptPolicy]]
[[Category:Civ5 Policies API|CanAdoptPolicy]]