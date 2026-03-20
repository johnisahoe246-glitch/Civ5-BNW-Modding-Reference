{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.ChangeNoNukesCount<b>(</b>'''int''' change<b>)</b></code>


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
{{CodeLine5|0325}}<syntaxhighlight lang="lua">Game:ChangeNoNukesCount(5 + iRandom);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeNoNukesCount]]
[[Category:Civ5 Combat API|ChangeNoNukesCount]]
[[Category:Civ5 Diplomacy API|ChangeNoNukesCount]]