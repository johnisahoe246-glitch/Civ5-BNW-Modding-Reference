{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.FoundPantheon<b>(</b>'''int''' vaticanPlayer, {{Type5|BeliefType}} belief1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|vaticanPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|belief1:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0845}}<syntaxhighlight lang="lua">Game.FoundPantheon(iVaticanPlayer, eBelief1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0855}}<syntaxhighlight lang="lua">Game.FoundPantheon(iMeccaPlayer, eBelief1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0872}}<syntaxhighlight lang="lua">Game.FoundPantheon(iPlayer, eBelief1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|FoundPantheon]]
[[Category:Civ5 Religion API|FoundPantheon]]