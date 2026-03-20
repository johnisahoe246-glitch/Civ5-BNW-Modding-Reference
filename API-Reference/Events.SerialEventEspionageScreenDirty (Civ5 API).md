{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventEspionageScreenDirty<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventEspionageScreenDirty.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventEspionageScreenDirty(''<arguments list>'')</code>.



=Source code samples=
{{PseudoH4|DiploCorner.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0410}}<syntaxhighlight lang="lua">Events.SerialEventEspionageScreenDirty.Add(DoUpdateEspionageButton);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1405}}<syntaxhighlight lang="lua">Events.SerialEventEspionageScreenDirty.Add(Refresh);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventEspionageScreenDirty]]