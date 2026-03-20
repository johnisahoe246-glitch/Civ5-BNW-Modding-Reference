{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|FileHeader}} PreGame.GetFileHeader<b>(</b>'''string''' path<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|path:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">header = PreGame.GetFileHeader( thisLoadFile, true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0055}}<syntaxhighlight lang="lua">header = PreGame.GetFileHeader( thisLoadFile );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0215}}<syntaxhighlight lang="lua">header = PreGame.GetFileHeader(g_FileList[g_iSelected]);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0170}}<syntaxhighlight lang="lua">entry.SaveData = PreGame.GetFileHeader(entry.FileName);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFileHeader]]