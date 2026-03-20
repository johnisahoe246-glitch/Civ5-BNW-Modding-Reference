{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.PlayerChoseToLoadGame<b>(</b>'''string''' thisLoadFile, '''bool''' arg1 = nil<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.PlayerChoseToLoadGame.Add(''<function handler>'')</code> or invoke it directly through <code>Events.PlayerChoseToLoadGame(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|thisLoadFile:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0033}}<syntaxhighlight lang="lua">Events.PlayerChoseToLoadGame(Steam.GetCloudSaveFileName(g_iSelected), true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">Events.PlayerChoseToLoadGame(thisLoadFile);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlayerChoseToLoadGame]]
[[Category:Civ5 Movement API|PlayerChoseToLoadGame]]
[[Category:Civ5 Players API|PlayerChoseToLoadGame]]