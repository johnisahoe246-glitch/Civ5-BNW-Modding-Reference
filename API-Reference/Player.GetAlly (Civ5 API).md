{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|PlayerID}} Player:GetAlly<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0534}}<syntaxhighlight lang="lua">local iAlly = pPlayer:GetAlly();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2581}}<syntaxhighlight lang="lua">local iAlly = pLoopPlayer:GetAlly();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2616}}<syntaxhighlight lang="lua">elseif (pLoopPlayer:IsMinorCiv() and pLoopPlayer:GetAlly() == iFromPlayer) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2987}}<syntaxhighlight lang="lua">local iAlly = Players[iOtherPlayer]:GetAlly();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0431}}<syntaxhighlight lang="lua">local iAlly = pVaticanPlayer:GetAlly();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1166}}<syntaxhighlight lang="lua">local iJerusalemAlly = pJerusalemPlayer:GetAlly();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0722}}<syntaxhighlight lang="lua">elseif(iPlayerLoop == curPlayer:GetAlly()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetAlly]]
[[Category:Civ5 Diplomacy API|GetAlly]]