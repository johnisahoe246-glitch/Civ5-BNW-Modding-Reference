{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' OptionsManager.SetFullscreen_Cached<b>(</b>'''bool''' fullscreen<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|fullscreen:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0181}}<syntaxhighlight lang="lua">OptionsManager.SetFullscreen_Cached(bFullscreen);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1022}}<syntaxhighlight lang="lua">OptionsManager.SetFullscreen_Cached( bIsChecked );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetFullscreen_Cached]]