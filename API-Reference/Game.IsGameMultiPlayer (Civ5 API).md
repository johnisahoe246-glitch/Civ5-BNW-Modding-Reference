{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.IsGameMultiPlayer<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0388}}<syntaxhighlight lang="lua">if( Game.IsGameMultiPlayer() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0215}}<syntaxhighlight lang="lua">if(g_pPlayer:GetNickName() ~= "" and Game.IsGameMultiPlayer()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0262}}<syntaxhighlight lang="lua">if(pOtherPlayer:GetNickName() ~= "" and Game.IsGameMultiPlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">if(Game.IsGameMultiPlayer()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">local isTutorialOrMultiplayer = Game and (Game.IsGameMultiPlayer() or Game.IsStaticTutorialActive());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0696}}<syntaxhighlight lang="lua">if( Game:IsGameMultiPlayer() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0130}}<syntaxhighlight lang="lua">if( Game.IsGameMultiPlayer() == false and bIsLocalPlayer ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">if( bMet or Game.IsGameMultiPlayer() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0370}}<syntaxhighlight lang="lua">if( Game.IsGameMultiPlayer() or OptionsManager.GetScoreList() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0548}}<syntaxhighlight lang="lua">if (Game:IsGameMultiPlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0542}}<syntaxhighlight lang="lua">if (Game.IsGameMultiPlayer() or Game.IsHotSeat()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsGameMultiPlayer]]
[[Category:Civ5 Players API|IsGameMultiPlayer]]