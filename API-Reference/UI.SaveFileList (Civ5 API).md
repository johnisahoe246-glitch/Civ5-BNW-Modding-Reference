{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.SaveFileList<b>(</b>table({{Type5|SpecialistType}} => '''bool''') FileList, {{Type5|GameType}} GameType, '''bool''' ShowAutoSaves, '''bool''' arg3<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|FileList:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|GameType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ShowAutoSaves:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg3:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0569}}<syntaxhighlight lang="lua">UI.SaveFileList( g_FileList, g_GameType, g_ShowAutoSaves, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0555}}<syntaxhighlight lang="lua">UI.SaveFileList( savedGames, gameType, false, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SaveFileList]]