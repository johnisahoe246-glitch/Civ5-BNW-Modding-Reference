{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetDLCAllowed<b>(</b>'''unknown''' arg0, '''bool''' check<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|check:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0996}}<syntaxhighlight lang="lua">PreGame.SetDLCAllowed(row.PackageID, bCheck);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1001}}<syntaxhighlight lang="lua">PreGame.SetDLCAllowed(row.PackageID, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetDLCAllowed]]
[[Category:Civ5 Game Settings API|SetDLCAllowed]]