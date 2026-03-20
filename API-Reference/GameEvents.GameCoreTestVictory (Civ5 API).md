{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' GameEvents.GameCoreTestVictory<b>(</b><b>)</b></code>


'''Event Type'''
:Unknown



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0050}}<syntaxhighlight lang="lua">GameEvents.GameCoreTestVictory.Remove(TestVictory);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0056}}<syntaxhighlight lang="lua">GameEvents.GameCoreTestVictory.Add(TestVictory);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GameCoreTestVictory]]
[[Category:Civ5 Victory API|GameCoreTestVictory]]