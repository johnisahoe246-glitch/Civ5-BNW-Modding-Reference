{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
<br/>
*This method was added in Gods & Kings.
}}


=Usage=
<code>'''void''' GameEvents.GetScenarioDiploModifier1<b>(</b>{{Type5|PlayerID}} player1, {{Type5|PlayerID}} player2<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player1:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|player2:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0457}}<syntaxhighlight lang="lua">GameEvents.GetScenarioDiploModifier1.Add(function(ePlayer1, ePlayer2)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0459}}<syntaxhighlight lang="lua">local eReligion1;</syntaxhighlight>
{{CodeLine5|0460}}<syntaxhighlight lang="lua">local eReligion2;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0462}}<syntaxhighlight lang="lua">eReligion1 = MyCurrentReligion(ePlayer1);</syntaxhighlight>
{{CodeLine5|0463}}<syntaxhighlight lang="lua">eReligion2 = MyCurrentReligion(ePlayer2);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0465}}<syntaxhighlight lang="lua">if (eReligion1 ~= eReligion2) then</syntaxhighlight>
{{CodeLine5|0466}}<syntaxhighlight lang="lua">return 60;</syntaxhighlight>
{{CodeLine5|0467}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0468}}<syntaxhighlight lang="lua">return 0;</syntaxhighlight>
{{CodeLine5|0469}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0470}}<syntaxhighlight lang="lua">end)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0473}}<syntaxhighlight lang="lua">-- GetFounderBenefitsReligion</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0475}}<syntaxhighlight lang="lua">function OnGetFounderBenefitsReligion(ePlayer)</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0537}}<syntaxhighlight lang="lua">GameEvents.GetScenarioDiploModifier1.Add(function(ePlayer1, ePlayer2)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0539}}<syntaxhighlight lang="lua">if (GetNumTokensOwned(ePlayer2) == 2) then</syntaxhighlight>
{{CodeLine5|0540}}<syntaxhighlight lang="lua">return 20;</syntaxhighlight>
{{CodeLine5|0541}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0543}}<syntaxhighlight lang="lua">return 0;</syntaxhighlight>
{{CodeLine5|0544}}<syntaxhighlight lang="lua">end)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0546}}<syntaxhighlight lang="lua">-- Large negative modifier when other player has more than 2 Titles (about to win)</syntaxhighlight>
{{CodeLine5|0547}}<syntaxhighlight lang="lua">GameEvents.GetScenarioDiploModifier2.Add(function(ePlayer1, ePlayer2)</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetScenarioDiploModifier1]]
[[Category:Civ5 Diplomacy API|GetScenarioDiploModifier1]]