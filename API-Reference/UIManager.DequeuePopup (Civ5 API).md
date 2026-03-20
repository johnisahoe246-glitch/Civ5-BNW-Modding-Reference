{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UIManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UIManager.DequeuePopup<b>(</b>{{Type5|Context}} ContextPtr<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|ContextPtr:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1172}}<syntaxhighlight lang="lua">UIManager:DequeuePopup( ContextPtr );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0053}}<syntaxhighlight lang="lua">UIManager:DequeuePopup(ContextPtr);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0693}}<syntaxhighlight lang="lua">UIManager:DequeuePopup(Controls.EmptyPopup);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EULA.lua}}
:<code>UI/FrontEnd/Modding/EULA.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">UIManager:DequeuePopup(   ContextPtr );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DequeuePopup]]