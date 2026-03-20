{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' UI.IsMapScenario<b>(</b>'''string''' mapScriptFileName<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|mapScriptFileName:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0219}}<syntaxhighlight lang="lua">if( UI.IsMapScenario(mapScriptFileName)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0349}}<syntaxhighlight lang="lua">if(UI.IsMapScenario(mapScriptFileName)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsMapScenario]]