{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UIManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UIManager.PopModal<b>(</b>{{Type5|Context}} ContextPtr<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|ContextPtr:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Advisors.lua}}
:<code>UI/InGame/WorldView/Advisors.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">UIManager:PopModal(ContextPtr);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChangePassword.lua}}
:<code>UI/InGame/ChangePassword.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0013}}<syntaxhighlight lang="lua">UIManager:PopModal( ContextPtr );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0377}}<syntaxhighlight lang="lua">UIManager:PopModal(Controls.DeleteConfirm);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0858}}<syntaxhighlight lang="lua">UIManager:PopModal(Controls.OptionsPopup);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PopModal]]