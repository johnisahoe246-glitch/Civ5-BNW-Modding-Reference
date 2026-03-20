{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.ModBrowserSetDeleteButtonState<b>(</b>..., '''bool''' arg1, '''string''' arg2 = nil<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.ModBrowserSetDeleteButtonState.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.ModBrowserSetDeleteButtonState(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|...:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0087}}<syntaxhighlight lang="lua">LuaEvents.ModBrowserSetDeleteButtonState(false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0743}}<syntaxhighlight lang="lua">LuaEvents.ModBrowserSetDeleteButtonState(true, true, Locale.Lookup("TXT_KEY_MODDING_UNSUBSCRIBE_MOD"));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0745}}<syntaxhighlight lang="lua">LuaEvents.ModBrowserSetDeleteButtonState(true, true, Locale.Lookup("TXT_KEY_MODDING_DELETEMOD"));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsBrowser.lua}}
:<code>UI/FrontEnd/Modding/ModsBrowser.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">LuaEvents.ModBrowserSetDeleteButtonState.Add(function(...)</syntaxhighlight>
{{CodeLine5|0068}}<syntaxhighlight lang="lua">SetButtonState(Controls.SmallButton1, Controls.SmallButton1Label, ...);</syntaxhighlight>
{{CodeLine5|0069}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ModBrowserSetDeleteButtonState]]