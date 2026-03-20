{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.DoFromUIDiploEvent<b>(</b>{{Type5|DiploUIEventType}} event, {{Type5|PlayerID}} aIPlayer, {{Type5|SpecialistType}} button, '''int''' againstPlayer, '''int''' arg3<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|event:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|aIPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|button:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|againstPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg3:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DeclareWarMovePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_DECLARES_WAR, Teams[eRivalTeam]:GetLeaderID(), 0, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DeclareWarRangeStrikePopup.lua}}
:<code>UI/InGame/PopupsGeneric/DeclareWarRangeStrikePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0051}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_DECLARES_WAR, rivalTeam:GetLeaderID(), 0, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0500}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_DISCUSSION_DONT_SETTLE, g_iAIPlayer, 0, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0515}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_AGGRESSIVE_MILITARY_WARNING_RESPONSE, g_iAIPlayer, iButtonID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0519}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_I_ATTACKED_YOUR_MINOR_CIV_RESPONSE, g_iAIPlayer, iButtonID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0523}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_ATTACKED_MINOR_RESPONSE, g_iAIPlayer, iButtonID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0535}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_EXPANSION_WARNING_RESPONSE, g_iAIPlayer, iButtonID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0543}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_PLOT_BUYING_WARNING_RESPONSE, g_iAIPlayer, iButtonID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0547}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_WORK_WITH_US_RESPONSE, g_iAIPlayer, iButtonID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0552}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_WORK_AGAINST_SOMEONE_RESPONSE, g_iAIPlayer, iButtonID, iAgainstPlayer );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0557}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_COOP_WAR_RESPONSE, g_iAIPlayer, iButtonID, iAgainstPlayer );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0562}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_COOP_WAR_NOW_RESPONSE, g_iAIPlayer, iButtonID, iAgainstPlayer );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0566}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_PLAN_RA_RESPONSE, g_iAIPlayer, iButtonID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0571}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_AI_REQUEST_DENOUNCE_RESPONSE, g_iAIPlayer, iButtonID, iAgainstPlayer );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0632}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_DISCUSSION_WORK_WITH_US, g_iAIPlayer, 0, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0955}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_COOP_WAR_OFFER, g_iAIPlayer, iLeaderId, -1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0971}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_DENOUNCE, g_iAIPlayer, 0, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0638}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_DISCUSSION_SHARE_INTRIGUE, g_iAIPlayer, iIntriguePlotter, iIntrigueType);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0658}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_I_ATTACKED_YOUR_MINOR_CIV_RESPONSE, g_iAIPlayer, iButtonID, iMinor );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0663}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_I_BULLIED_YOUR_MINOR_CIV_RESPONSE, g_iAIPlayer, iButtonID, iMinor );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0675}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_BULLIED_MINOR_RESPONSE, g_iAIPlayer, iButtonID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0723}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_CAUGHT_YOUR_SPY_RESPONSE, g_iAIPlayer, iButtonID, iAgainstPlayer);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0731}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_KILLED_MY_SPY_RESPONSE, g_iAIPlayer, iButtonID, iAgainstPlayer);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0736}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_KILLED_MY_SPY_RESPONSE, g_iAIPlayer, 2, iAgainstPlayer);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0740}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_STOP_CONVERSIONS, g_iAIPlayer, iButtonID, iAgainstPlayer);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0800}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_DISCUSSION_STOP_SPYING, g_iAIPlayer, 0, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0898}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_DISCUSSION_STOP_SPYING, g_iAIPlayer, 1, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1244}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_DECLARES_WAR, g_iAIPlayer, 1, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LeaderHeadRoot.lua}}
:<code>UI/InGame/LeaderHead/LeaderHeadRoot.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0234}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_WANTS_DISCUSSION, g_iAIPlayer, 0, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0271}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_NEGOTIATE_PEACE, g_iAIPlayer, 0, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0310}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_HUMAN_DECLARES_WAR, g_iAIPlayer, 0, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0369}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_DEMAND_HUMAN_REFUSAL, g_iThem, 0, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0371}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_REQUEST_HUMAN_REFUSAL, g_iThem, 0, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0400}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_KILLED_MINOR_RESPONSE, g_iThem, iButtonID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0403}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_EXPANSION_SERIOUS_WARNING_RESPONSE, g_iThem, iButtonID, 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0406}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_PLOT_BUYING_SERIOUS_WARNING_RESPONSE, g_iThem, iButtonID, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0374}}<syntaxhighlight lang="lua">Game.DoFromUIDiploEvent( FromUIDiploEventTypes.FROM_UI_DIPLO_EVENT_REQUEST_HUMAN_REFUSAL, g_iThem, iDealValue, 0 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DoFromUIDiploEvent]]
[[Category:Civ5 Diplomacy API|DoFromUIDiploEvent]]