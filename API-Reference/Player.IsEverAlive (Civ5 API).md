{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:IsEverAlive<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">if (pPlayer:IsEverAlive() and pPlayer:HasCreatedReligion()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0654}}<syntaxhighlight lang="lua">if player:IsEverAlive() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1280}}<syntaxhighlight lang="lua">if(player and player:IsEverAlive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0468}}<syntaxhighlight lang="lua">if (pLoopPlayer:IsEverAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2767}}<syntaxhighlight lang="lua">if( pLoopPlayer:IsEverAlive() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0217}}<syntaxhighlight lang="lua">if(not pPlayer:IsMinorCiv() and pPlayer:IsEverAlive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0259}}<syntaxhighlight lang="lua">if(pPlayer:IsEverAlive()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsEverAlive]]
[[Category:Civ5 Players API|IsEverAlive]]