{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetRandomWorldSize<b>(</b>'''bool''' arg0<b>)</b></code>


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
{{CodeLine5|0603}}<syntaxhighlight lang="lua">PreGame.SetRandomWorldSize( true );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0609}}<syntaxhighlight lang="lua">PreGame.SetRandomWorldSize( false );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0800}}<syntaxhighlight lang="lua">PreGame.SetRandomWorldSize(false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">PreGame.SetRandomWorldSize(true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetRandomWorldSize]]
[[Category:Civ5 Game Settings API|SetRandomWorldSize]]