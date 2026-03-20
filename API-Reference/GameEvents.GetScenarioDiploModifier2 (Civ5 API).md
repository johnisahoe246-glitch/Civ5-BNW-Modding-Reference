{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
<br/>
*This method was added in Gods & Kings.
}}


=Usage=
<code>'''void''' GameEvents.GetScenarioDiploModifier2<b>(</b>{{Type5|PlayerID}} player1, {{Type5|PlayerID}} player2<b>)</b></code>


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
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0547}}<syntaxhighlight lang="lua">GameEvents.GetScenarioDiploModifier2.Add(function(ePlayer1, ePlayer2)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0549}}<syntaxhighlight lang="lua">if (GetNumTokensOwned(ePlayer2) > 2) then</syntaxhighlight>
{{CodeLine5|0550}}<syntaxhighlight lang="lua">return 70;</syntaxhighlight>
{{CodeLine5|0551}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0553}}<syntaxhighlight lang="lua">return 0;</syntaxhighlight>
{{CodeLine5|0554}}<syntaxhighlight lang="lua">end)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0556}}<syntaxhighlight lang="lua">function CanAdoptPolicyBranch (iPlayerID, iPolicyBranch)</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetScenarioDiploModifier2]]
[[Category:Civ5 Diplomacy API|GetScenarioDiploModifier2]]