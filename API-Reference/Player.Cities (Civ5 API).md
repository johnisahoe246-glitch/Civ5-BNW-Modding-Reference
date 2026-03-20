{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


Returns all of a player's cities. Must be used in a for loop because it's an iterator function (see example)


=Usage=
<code>iterator({{Type5|City}}) Player:Cities<b>(</b><b>)</b></code>


'''Returned Value'''
:Iterator over all of a player's cities


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
for City in Player:Cities() do
...
end
local pPlayer = Players[Game.GetActivePlayer()]
for pCity in pPlayer:Cities() do
print("City ID ",pCity:GetID()," Population is ",pCity:GetPopulation())
end</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0100}}<syntaxhighlight lang="lua">for pCity in pPlayer:Cities() do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0197}}<syntaxhighlight lang="lua">for pCity in player:Cities() do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1267}}<syntaxhighlight lang="lua">for pCity in g_pUs:Cities() do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1285}}<syntaxhighlight lang="lua">for pCity in g_pThem:Cities() do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2463}}<syntaxhighlight lang="lua">for pCity in m_pFrom:Cities() do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0414}}<syntaxhighlight lang="lua">for pCity in Players[playerID]:Cities() do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0257}}<syntaxhighlight lang="lua">for v in player:Cities() do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2524}}<syntaxhighlight lang="lua">for v in pOtherPlayer:Cities() do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2750}}<syntaxhighlight lang="lua">for v in pPlayer:Cities() do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WhosWinningPopup.lua}}
:<code>UI/InGame/Popups/WhosWinningPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0192}}<syntaxhighlight lang="lua">for pLoopCity in pPlayer:Cities() do</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Cities]]
[[Category:Civ5 Cities API|Cities]]