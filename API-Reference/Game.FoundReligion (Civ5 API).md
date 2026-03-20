{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.FoundReligion<b>(</b>{{Type5|PlayerID}} vaticanPlayer, {{Type5|ReligionType}} religion, '''unknown''' arg2, {{Type5|BeliefType}} belief2, {{Type5|BeliefType}} belief3, {{Type5|BeliefType}} belief3, '''int''' arg6, {{Type5|City}} vaticanCity<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|vaticanPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|religion:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|belief2:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|belief3:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|belief3:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg6:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|vaticanCity:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0846}}<syntaxhighlight lang="lua">Game.FoundReligion(iVaticanPlayer, eReligion, nil, eBelief2, eBelief3, -1, -1, pVaticanCity);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0856}}<syntaxhighlight lang="lua">Game.FoundReligion(iMeccaPlayer, eReligion, nil, eBelief2, eBelief3, -1, -1, pMeccaCity);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0873}}<syntaxhighlight lang="lua">Game.FoundReligion(iPlayer, eReligion, nil, eBelief2, eBelief3, -1, -1, capital);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1479}}<syntaxhighlight lang="lua">Game.FoundReligion(iPlayer, eReligion, nil, eBelief1, eBelief2, eBelief3, -1, pBestCity);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|FoundReligion]]
[[Category:Civ5 Religion API|FoundReligion]]