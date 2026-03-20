{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|PlayerID}} Team:GetLeaderID<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DeclareWarMovePopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">local iMinor = Teams[eRivalTeam]:GetLeaderID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_DECLARES_WAR, Teams[eRivalTeam]:GetLeaderID(), 0, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarRangeStrikePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarRangeStrikePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">local iMinor = rivalTeam:GetLeaderID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0051}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_DECLARES_WAR, rivalTeam:GetLeaderID(), 0, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">iPlayerLoop = pOtherTeam:GetLeaderID();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0271}}<syntaxhighlight lang="lua">index = team:GetLeaderID();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0371}}<syntaxhighlight lang="lua">local pPlayer = Players[UNHome:GetLeaderID()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0700}}<syntaxhighlight lang="lua">local iLeader = v:GetLeaderID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0702}}<syntaxhighlight lang="lua">local curPlayer = Players[v:GetLeaderID()];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0677}}<syntaxhighlight lang="lua">local iLeader = pTeam:GetLeaderID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0714}}<syntaxhighlight lang="lua">local iLeaderLoop = pTeamLoop:GetLeaderID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0784}}<syntaxhighlight lang="lua">local iLastVoteLeader = Teams[iPreviousVoteCast]:GetLeaderID();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">local pPlayer = Players[pTeam:GetLeaderID()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0106}}<syntaxhighlight lang="lua">local iVoteCastPlayer = pVoteCastTeam:GetLeaderID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">CivIconHookup( pVoteCastTeam:GetLeaderID(), 32, controlTable.BallotIcon, controlTable.BallotIconBG, controlTable.BallotIconShadow, false, true );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetLeaderID]]
[[Category:Civ5 Players API|GetLeaderID]]