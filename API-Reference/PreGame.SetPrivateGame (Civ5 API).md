{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetPrivateGame<b>(</b>'''int''' checked<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|checked:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0078}}<syntaxhighlight lang="lua">PreGame.SetPrivateGame( bChecked );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SinglePlayer.lua}}
:<code>UI/FrontEnd/SinglePlayer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">PreGame.SetPrivateGame(false);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetPrivateGame]]