{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' OptionsManager.SetResolution_Cached<b>(</b>{{Type5|EraType}} fullscreenRes<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|fullscreenRes:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0178}}<syntaxhighlight lang="lua">OptionsManager.SetResolution_Cached(fullscreenRes);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1127}}<syntaxhighlight lang="lua">OptionsManager.SetResolution_Cached( index );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetResolution_Cached]]