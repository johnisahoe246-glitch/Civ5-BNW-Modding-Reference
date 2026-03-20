{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetScore<b>(</b>'''bool''' arg0 = nil, '''bool''' winner = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|winner:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0186}}<syntaxhighlight lang="lua">local strMyScore = g_pPlayer:GetScore();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0339}}<syntaxhighlight lang="lua">controlTable.Score:SetText( pOtherPlayer:GetScore() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0193}}<syntaxhighlight lang="lua">local strScore = pOtherPlayer:GetScore();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0175}}<syntaxhighlight lang="lua">controlTable.Score:SetText( pPlayer:GetScore() );</syntaxhighlight>
{{CodeLine5|0176}}<syntaxhighlight lang="lua">g_SortTable[ tostring( controlTable.Root ) ] = pPlayer:GetScore();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ranking.lua}}
:<code>UI/InGame/Popups/Ranking.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">local pPlayerScore = pPlayer:GetScore(true, bWinner);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">if (player:GetScore() >= 1000) then</syntaxhighlight>
{{CodeLine5|0019}}<syntaxhighlight lang="lua">print(string.format("Player %i has won w/ a score of %i", iPlayerLoop, player:GetScore()));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0032}}<syntaxhighlight lang="lua">if (player:GetScore() > iHighestScore) then</syntaxhighlight>
{{CodeLine5|0033}}<syntaxhighlight lang="lua">iHighestScore = player:GetScore();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0184}}<syntaxhighlight lang="lua">Controls.Score:SetText(pPlayer:GetScore());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0517}}<syntaxhighlight lang="lua">table.sort(sortedPlayerList, function(a, b) return Players[b]:GetScore() < Players[a]:GetScore() end);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0538}}<syntaxhighlight lang="lua">controlTable.Score:SetText(pPlayer:GetScore());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetScore]]
[[Category:Civ5 Score API|GetScore]]