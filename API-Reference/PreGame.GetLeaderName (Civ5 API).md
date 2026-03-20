{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''string''' PreGame.GetLeaderName<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0342}}<syntaxhighlight lang="lua">local name = PreGame.GetLeaderName(0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0217}}<syntaxhighlight lang="lua">elseif(PreGame.GetLeaderName(g_iPlayer) ~= "") then</syntaxhighlight>
{{CodeLine5|0218}}<syntaxhighlight lang="lua">TruncateString(Controls.LeaderName, textBoxSize, Locale.ConvertTextKey( PreGame.GetLeaderName( g_iPlayer ) ), "  (" .. Locale.ConvertTextKey( "TXT_KEY_YOU" ) .. ")");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">if(PreGame.GetLeaderName(Game.GetActivePlayer()) ~= "") then</syntaxhighlight>
{{CodeLine5|0076}}<syntaxhighlight lang="lua">TruncateString(controlTable.ButtonText, textBoxSize, Locale.ConvertTextKey( PreGame.GetLeaderName( Game.GetActivePlayer() ) ), "  (" .. Locale.ConvertTextKey( "TXT_KEY_YOU" ) .. ")");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0212}}<syntaxhighlight lang="lua">Controls.LeaderFrame:SetToolTipString( PreGame.GetLeaderName( 0 ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0329}}<syntaxhighlight lang="lua">TruncateString(Controls.DetailsLeader, availableTextExtent, PreGame.GetLeaderName(0));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameplayUtilities.lua}}
:<code>Gameplay/Lua/GameplayUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">elseif(PreGame.GetLeaderName(playerID) ~= "") then</syntaxhighlight>
{{CodeLine5|0024}}<syntaxhighlight lang="lua">name = PreGame.GetLeaderName(playerID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlayerChange.lua}}
:<code>UI/InGame/PlayerChange.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0091}}<syntaxhighlight lang="lua">szName = PreGame.GetLeaderName( eActivePlayer );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">PreGame.GetLeaderName(iPlayer),PreGame.GetCivilizationDescription(iPlayer), Players[iPlayer]:GetCurrentEra(), PreGame.GetGameType() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0196}}<syntaxhighlight lang="lua">PreGame.GetLeaderName(iPlayer), PreGame.GetCivilizationDescription(iPlayer), Players[iPlayer]:GetCurrentEra(), PreGame.GetGameType() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0627}}<syntaxhighlight lang="lua">local leaderName = PreGame.GetLeaderName(iPlayer);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0215}}<syntaxhighlight lang="lua">local name = PreGame.GetLeaderName(g_EditSlot);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetLeaderName]]
[[Category:Civ5 Players API|GetLeaderName]]