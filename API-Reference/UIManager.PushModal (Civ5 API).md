{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UIManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UIManager.PushModal<b>(</b>{{Type5|Context}} ContextPtr, '''bool''' arg1 = nil<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|ContextPtr:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1118}}<syntaxhighlight lang="lua">UIManager:PushModal(Controls.SetCivNames);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Advisors.lua}}
:<code>UI/InGame/WorldView/Advisors.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0247}}<syntaxhighlight lang="lua">UIManager:PushModal(ContextPtr, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ExitConfirm.lua}}
:<code>UI/FrontEnd/ExitConfirm.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">UIManager:PushModal( ContextPtr );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">UIManager:PushModal( Controls.SetCivNames );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0374}}<syntaxhighlight lang="lua">UIManager:PushModal(Controls.DeleteConfirm);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0853}}<syntaxhighlight lang="lua">UIManager:PushModal(Controls.OptionsPopup);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlayerChange.lua}}
:<code>UI/InGame/PlayerChange.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">UIManager:PushModal(Controls.ChangePassword, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0035}}<syntaxhighlight lang="lua">UIManager:PushModal( Controls.SaveMenu, false );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PushModal]]