{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|TeamID}} Team:GetID<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0224}}<syntaxhighlight lang="lua">Controls.TeamID:LocalizeAndSetText( "TXT_KEY_MULTIPLAYER_DEFAULT_TEAM_NAME", g_pTeam:GetID() + 1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0282}}<syntaxhighlight lang="lua">controlTable.TeamID:LocalizeAndSetText( "TXT_KEY_MULTIPLAYER_DEFAULT_TEAM_NAME", pOtherTeam:GetID() + 1 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0072}}<syntaxhighlight lang="lua">elseif(pOtherTeam:GetID() == pTeam:GetID())then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0081}}<syntaxhighlight lang="lua">TruncateString(controlTable.ButtonText, textBoxSize, Locale.ConvertTextKey("TXT_KEY_POP_UN_TEAM_LABEL", pOtherTeam:GetID() + 1) , " (" .. Locale.ConvertTextKey("TXT_KEY_POP_VOTE_RESULTS_YOUR_TEAM") .. ")");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">TruncateString(controlTable.ButtonText, textBoxSize, Locale.ConvertTextKey("TXT_KEY_POP_UN_TEAM_LABEL", pOtherTeam:GetID() + 1));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0062}}<syntaxhighlight lang="lua">if (pOtherTeam:GetID() ~= pTeam:GetID()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0554}}<syntaxhighlight lang="lua">if (pPlot:IsRevealed(pTeam:GetID())) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">item.TeamID:LocalizeAndSetText( "TXT_KEY_MULTIPLAYER_DEFAULT_TEAM_NAME", pTeam:GetID() + 1 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">if ((pPlayer:GetID() == activePlayer:GetID()) or (activePlayer:GetTeam() == pTeam:GetID())) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">strName = strName .. " " .. Locale.ConvertTextKey("TXT_KEY_POP_UN_TEAM_LABEL", pTeam:GetID() + 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0139}}<syntaxhighlight lang="lua">strVote = Locale.ConvertTextKey("TXT_KEY_POP_UN_TEAM_LABEL", pVoteCastTeam:GetID() + 1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetID]]