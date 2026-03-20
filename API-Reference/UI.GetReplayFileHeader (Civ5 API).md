{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|FileHeader}} UI.GetReplayFileHeader<b>(</b>'''unknown''' arg0<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|LoadReplayMenu.lua}}
:<code>UI/FrontEnd/LoadReplayMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0141}}<syntaxhighlight lang="lua">local header = UI.GetReplayFileHeader(g_FileList[g_iSelected]);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetReplayFileHeader]]