{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>'''void''' ChangeBuildingSize<b>(</b>'''float''' arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0392}}<syntaxhighlight lang="lua">ChangeBuildingSize( 0.01 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0395}}<syntaxhighlight lang="lua">ChangeBuildingSize( -0.01 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeBuildingSize]]
[[Category:Civ5 Buildings API|ChangeBuildingSize]]