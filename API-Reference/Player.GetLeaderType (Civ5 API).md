{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|LeaderType}} Player:GetLeaderType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">local otherLeaderType = pOtherPlayer:GetLeaderType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0207}}<syntaxhighlight lang="lua">local myLeaderType = g_pPlayer:GetLeaderType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">local leaderType = pOtherPlayer:GetLeaderType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0065}}<syntaxhighlight lang="lua">local leader = GameInfo.Leaders[pOtherPlayer:GetLeaderType()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0060}}<syntaxhighlight lang="lua">local otherLeader = GameInfo.Leaders[player:GetLeaderType()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0188}}<syntaxhighlight lang="lua">local leader = GameInfo.Leaders[pPlayer:GetLeaderType()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameplayUtilities.lua}}
:<code>Gameplay/Lua/GameplayUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">local leaderID = player:GetLeaderType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LeaderHeadRoot.lua}}
:<code>UI/InGame/LeaderHead/LeaderHeadRoot.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0044}}<syntaxhighlight lang="lua">playerLeaderInfo = GameInfo.Leaders[player:GetLeaderType()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlayerChange.lua}}
:<code>UI/InGame/PlayerChange.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0095}}<syntaxhighlight lang="lua">local leaderType = pPlayer:GetLeaderType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1284}}<syntaxhighlight lang="lua">Leader = GameInfo.Leaders[player:GetLeaderType()].Type,</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0960}}<syntaxhighlight lang="lua">local themLeaderType = g_pThem:GetLeaderType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryStatus.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryStatus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0126}}<syntaxhighlight lang="lua">local tLeader = GameInfo.Leaders[pPlayer:GetLeaderType()];</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetLeaderType]]
[[Category:Civ5 Players API|GetLeaderType]]