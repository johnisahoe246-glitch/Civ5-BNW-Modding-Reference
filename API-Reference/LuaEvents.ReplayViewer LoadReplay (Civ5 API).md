{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.ReplayViewer_LoadReplay<b>(</b>'''unknown''' replayFile<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.ReplayViewer_LoadReplay.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.ReplayViewer_LoadReplay(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|replayFile:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|LoadReplayMenu.lua}}
:<code>UI/FrontEnd/LoadReplayMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">LuaEvents.ReplayViewer_LoadReplay(replayFile);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1240}}<syntaxhighlight lang="lua">LuaEvents.ReplayViewer_LoadReplay.Add(function(file)</syntaxhighlight>
{{CodeLine5|1241}}<syntaxhighlight lang="lua">print("Loading Replay - " .. file);</syntaxhighlight>
{{CodeLine5|1242}}<syntaxhighlight lang="lua">g_ReplayInfo = UI.GetReplayInfo(file);</syntaxhighlight>
{{CodeLine5|1243}}<syntaxhighlight lang="lua">Refresh();</syntaxhighlight>
{{CodeLine5|1244}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ReplayViewer_LoadReplay]]
[[Category:Civ5 Movement API|ReplayViewer_LoadReplay]]