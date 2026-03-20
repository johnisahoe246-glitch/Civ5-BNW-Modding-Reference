{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' OptionsManager.GetFullscreen_Cached<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0172}}<syntaxhighlight lang="lua">bFullscreen = OptionsManager.GetFullscreen_Cached();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0724}}<syntaxhighlight lang="lua">local bIsFullscreen = OptionsManager.GetFullscreen_Cached();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFullscreen_Cached]]