{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:IsHuman<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0242}}<syntaxhighlight lang="lua">if(otherPlayer:IsHuman() and otherPlayer:IsTurnActive()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1077}}<syntaxhighlight lang="lua">if player:IsHuman() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0331}}<syntaxhighlight lang="lua">if( iPlayer ~= g_iLocalPlayer and pPlayer ~= nil and pPlayer:IsHuman() and pPlayer:GetTeam() == g_iLocalTeam ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0350}}<syntaxhighlight lang="lua">if( iPlayer ~= g_iLocalPlayer and pPlayer ~= nil and pPlayer:IsHuman() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">if( pOtherPlayer:GetNickName() ~= "" and pOtherPlayer:IsHuman() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0060}}<syntaxhighlight lang="lua">if (pOtherPlayer:IsHuman()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0160}}<syntaxhighlight lang="lua">if (pThirdPlayer:IsHuman()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">elseif (pThirdPlayer:IsHuman()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0325}}<syntaxhighlight lang="lua">if (Players[ ePlayer ]:IsHuman()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0133}}<syntaxhighlight lang="lua">if( Players[ePlayer]:IsHuman() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0308}}<syntaxhighlight lang="lua">elseif (pOtherPlayer:IsHuman() or pOtherTeam:IsHuman()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0345}}<syntaxhighlight lang="lua">if( pOtherPlayer:IsHuman() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0202}}<syntaxhighlight lang="lua">if(pOtherPlayer:GetNickName() ~= "" and pOtherPlayer:IsHuman()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0211}}<syntaxhighlight lang="lua">if (activePlayer:HasRecentIntrigueAbout(iPlayer) and not Players[iPlayer]:IsHuman()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">if (iActivePlayer ~= iNextPlayer and pPlayer:IsAlive() and pPlayer:IsHuman()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0086}}<syntaxhighlight lang="lua">if (pPlayer:IsAlive() and pPlayer:IsHuman()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0105}}<syntaxhighlight lang="lua">local bIsHuman = pPlayer:IsHuman();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NewTurn.lua}}
:<code>UI/InGame/NewTurn.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0017}}<syntaxhighlight lang="lua">if (not Players[iPlayerID]:IsHuman()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceIconManager.lua}}
:<code>UI/InGame/ResourceIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0083}}<syntaxhighlight lang="lua">if( pPlayer ~= nil and pPlayer:IsHuman() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReturnCivilianPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ReturnCivilianPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">elseif (not pGiftedPlayer:IsHuman()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2773}}<syntaxhighlight lang="lua">if( pLoopPlayer:IsHuman() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialInclude_Expansion1.lua (G&K)}}
:<code>DLC/Expansion/Tutorial/TutorialInclude_Expansion1.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">if (player ~= nil and player:IsHuman()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1575}}<syntaxhighlight lang="lua">if (pPlayer:IsHuman()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsHuman]]
[[Category:Civ5 Players API|IsHuman]]