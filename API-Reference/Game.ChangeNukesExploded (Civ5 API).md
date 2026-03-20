{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.ChangeNukesExploded<b>(</b>'''int''' change<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|change:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0199}}<syntaxhighlight lang="lua">Game:ChangeNukesExploded(1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeNukesExploded]]
[[Category:Civ5 Combat API|ChangeNukesExploded]]
[[Category:Civ5 Diplomacy API|ChangeNukesExploded]]