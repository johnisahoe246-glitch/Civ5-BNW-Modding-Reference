{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''unknown''' UI.GetVersionInfo<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0005}}<syntaxhighlight lang="lua">Controls.VersionNumber_Label:SetText(UI.GetVersionInfo());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MainMenu.lua}}
:<code>UI/FrontEnd/MainMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">local i1, i2 = string.find( UI.GetVersionInfo(), " " );</syntaxhighlight>
{{CodeLine5|0013}}<syntaxhighlight lang="lua">versionNumber = string.sub(UI.GetVersionInfo(), 1, i2-1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetVersionInfo]]