{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.IsNetworkMultiPlayer<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DeclareWarMovePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0074}}<syntaxhighlight lang="lua">if (not Game.IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0008}}<syntaxhighlight lang="lua">local m_bIsMultiplayer = Game:IsNetworkMultiPlayer();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">if(pOtherPlayer:GetNickName() ~= "" and Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0198}}<syntaxhighlight lang="lua">if(pAIPlayer:GetNickName() ~= "" and Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0180}}<syntaxhighlight lang="lua">if (not Game:IsNetworkMultiPlayer() and player:IsAlive() and PreGame.GetGameOption("GAMEOPTION_NO_EXTENDED_PLAY") ~= 1) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0878}}<syntaxhighlight lang="lua">if(pPlayer:GetNickName() ~= "" and Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0097}}<syntaxhighlight lang="lua">if (Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0138}}<syntaxhighlight lang="lua">if(Game.IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">if(Game:IsNetworkMultiPlayer() and pPlayer:GetNickName() ~= "") then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameplayUtilities.lua}}
:<code>Gameplay/Lua/GameplayUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0021}}<syntaxhighlight lang="lua">if(nickName and #nickName > 0 and Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0021}}<syntaxhighlight lang="lua">local g_ShowWorkerRecommendation = not Game.IsNetworkMultiPlayer();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0697}}<syntaxhighlight lang="lua">if( Game:IsNetworkMultiPlayer() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0078}}<syntaxhighlight lang="lua">if( ContextPtr:IsHidden() == false and Game.IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0107}}<syntaxhighlight lang="lua">local bIsNetworkMP = Game.IsNetworkMultiPlayer();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMapMenu.lua}}
:<code>UI/InGame/Menus/SaveMapMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0279}}<syntaxhighlight lang="lua">g_IsSingle = not Game:IsNetworkMultiPlayer();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0617}}<syntaxhighlight lang="lua">if( Game:IsNetworkMultiPlayer() or</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0457}}<syntaxhighlight lang="lua">if (Teams[leadAI:GetTeam()]:IsHasMet(Game.GetActiveTeam()) or Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeLine5|0458}}<syntaxhighlight lang="lua">if(leadAI:GetNickName() ~= "" and Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0837}}<syntaxhighlight lang="lua">if (pTeam:IsHasMet(Game.GetActiveTeam()) or Game:IsNetworkMultiPlayer()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsNetworkMultiPlayer]]
[[Category:Civ5 Players API|IsNetworkMultiPlayer]]