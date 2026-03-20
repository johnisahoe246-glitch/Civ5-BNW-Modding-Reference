{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' OptionsManager.GetPolicyInfo<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">local bShowAll = OptionsManager.GetPolicyInfo();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0544}}<syntaxhighlight lang="lua">if (bIsChecked ~= OptionsManager.GetPolicyInfo()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0921}}<syntaxhighlight lang="lua">Controls.PolicyInfo:SetCheck( OptionsManager.GetPolicyInfo() );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPolicyInfo]]
[[Category:Civ5 Policies API|GetPolicyInfo]]