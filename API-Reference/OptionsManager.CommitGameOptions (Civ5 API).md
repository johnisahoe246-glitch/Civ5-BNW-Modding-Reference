{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' OptionsManager.CommitGameOptions<b>(</b>'''int''' arg0 = nil<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0128}}<syntaxhighlight lang="lua">OptionsManager.CommitGameOptions(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0318}}<syntaxhighlight lang="lua">OptionsManager.CommitGameOptions( PreGame.IsHotSeatGame() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0369}}<syntaxhighlight lang="lua">OptionsManager.CommitGameOptions(PreGame.IsHotSeatGame());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">OptionsManager.CommitGameOptions();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CommitGameOptions]]
[[Category:Civ5 Game Settings API|CommitGameOptions]]