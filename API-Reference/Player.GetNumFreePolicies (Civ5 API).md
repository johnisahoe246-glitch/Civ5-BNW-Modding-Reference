{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNumFreePolicies<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0269}}<syntaxhighlight lang="lua">local iNumFreePolicies = player:GetNumFreePolicies();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumFreePolicies]]
[[Category:Civ5 Policies API|GetNumFreePolicies]]