{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' OptionsManager.SetWindowResolution_Cached<b>(</b>'''int''' arg0, '''int''' arg1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0179}}<syntaxhighlight lang="lua">OptionsManager.SetWindowResolution_Cached(windowedRes[1], windowedRes[2]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1114}}<syntaxhighlight lang="lua">OptionsManager.SetWindowResolution_Cached( kResInfo.x, kResInfo.y );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1130}}<syntaxhighlight lang="lua">OptionsManager.SetWindowResolution_Cached( kResInfo.Width, kResInfo.Height );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetWindowResolution_Cached]]