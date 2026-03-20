{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Player:AddTemporaryDominanceZone<b>(</b>'''int''' arg0, '''int''' arg1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0579}}<syntaxhighlight lang="lua">player:AddTemporaryDominanceZone (41, 10);  -- Chichester</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0581}}<syntaxhighlight lang="lua">player:AddTemporaryDominanceZone (36, 10);  -- Wareham</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0583}}<syntaxhighlight lang="lua">player:AddTemporaryDominanceZone (30, 9);  -- Exeter</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0629}}<syntaxhighlight lang="lua">player:AddTemporaryDominanceZone (49, 26);  -- Norwich</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0631}}<syntaxhighlight lang="lua">player:AddTemporaryDominanceZone (49, 21);  -- Ipswich</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0633}}<syntaxhighlight lang="lua">player:AddTemporaryDominanceZone (48, 13);  -- Dover</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0677}}<syntaxhighlight lang="lua">player:AddTemporaryDominanceZone (33, 30);  -- Chester</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0721}}<syntaxhighlight lang="lua">player:AddTemporaryDominanceZone (48,13);  -- Dover</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0765}}<syntaxhighlight lang="lua">norway:AddTemporaryDominanceZone (40, 36);  -- York</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1662}}<syntaxhighlight lang="lua">Players[iPlayer]:AddTemporaryDominanceZone (48, 7);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1706}}<syntaxhighlight lang="lua">Players[iPlayer]:AddTemporaryDominanceZone (71, 9);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1750}}<syntaxhighlight lang="lua">Players[iPlayer]:AddTemporaryDominanceZone (68, 20);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1794}}<syntaxhighlight lang="lua">Players[iPlayer]:AddTemporaryDominanceZone (49, 18);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1834}}<syntaxhighlight lang="lua">Players[iPlayer]:AddTemporaryDominanceZone (54, 31);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1875}}<syntaxhighlight lang="lua">Players[iPlayer]:AddTemporaryDominanceZone (49, 34);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1916}}<syntaxhighlight lang="lua">Players[iPlayer]:AddTemporaryDominanceZone (45, 35);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1957}}<syntaxhighlight lang="lua">Players[iPlayer]:AddTemporaryDominanceZone (75, 34);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2001}}<syntaxhighlight lang="lua">Players[iPlayer]:AddTemporaryDominanceZone (78, 32);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2045}}<syntaxhighlight lang="lua">Players[iPlayer]:AddTemporaryDominanceZone (17, 52);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2089}}<syntaxhighlight lang="lua">Players[iPlayer]:AddTemporaryDominanceZone (22, 53);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2135}}<syntaxhighlight lang="lua">Players[iPlayer]:AddTemporaryDominanceZone (26, 49);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2179}}<syntaxhighlight lang="lua">Players[iPlayer]:AddTemporaryDominanceZone (32, 45);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AddTemporaryDominanceZone]]