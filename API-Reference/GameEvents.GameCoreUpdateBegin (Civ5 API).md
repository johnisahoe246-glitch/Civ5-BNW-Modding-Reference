{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}

This event fires about once every 100ms.

=Usage=
<code>'''void''' GameEvents.GameCoreUpdateBegin<b>(</b><b>)</b></code>


'''Event Type'''
:Unknown



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0113}}<syntaxhighlight lang="lua">GameEvents.GameCoreUpdateBegin.Remove(OnGameCoreUpdateBegin);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">GameEvents.GameCoreUpdateBegin.Add(OnGameCoreUpdateBegin);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0139}}<syntaxhighlight lang="lua">GameEvents.GameCoreUpdateBegin.Add( OnGameCoreUpdateBegin );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GameCoreUpdateBegin]]