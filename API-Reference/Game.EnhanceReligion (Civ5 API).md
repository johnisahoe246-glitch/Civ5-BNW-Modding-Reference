{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.EnhanceReligion<b>(</b>{{Type5|PlayerID}} vaticanPlayer, {{Type5|ReligionType}} religion, {{Type5|BeliefType}} belief4, {{Type5|BeliefType}} belief5<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|vaticanPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|religion:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|belief4:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|belief5:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0847}}<syntaxhighlight lang="lua">Game.EnhanceReligion(iVaticanPlayer, eReligion, eBelief4, eBelief5);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0857}}<syntaxhighlight lang="lua">Game.EnhanceReligion(iMeccaPlayer, eReligion, eBelief4, eBelief5);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0874}}<syntaxhighlight lang="lua">Game.EnhanceReligion(iPlayer, eReligion, eBelief4, eBelief5);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|EnhanceReligion]]
[[Category:Civ5 Religion API|EnhanceReligion]]