{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetRandomMapScript<b>(</b>'''bool''' arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0780}}<syntaxhighlight lang="lua">PreGame.SetRandomMapScript(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0785}}<syntaxhighlight lang="lua">PreGame.SetRandomMapScript(false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0133}}<syntaxhighlight lang="lua">PreGame.SetRandomMapScript(false);   -- Random map scripts is not supported in multiplayer</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetRandomMapScript]]
[[Category:Civ5 Game Settings API|SetRandomMapScript]]