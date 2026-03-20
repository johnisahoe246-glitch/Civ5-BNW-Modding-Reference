{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetMinorCivFriendshipWithMajor<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|major:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0411}}<syntaxhighlight lang="lua">SetUpMinorMeter( player:GetMinorCivFriendshipWithMajor( iActivePlayer ), controls, textColor );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0494}}<syntaxhighlight lang="lua">elseif (player:GetMinorCivFriendshipWithMajor(iActivePlayer) < 0) then      -- Angry</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0549}}<syntaxhighlight lang="lua">if (Players[iMinor]:GetMinorCivFriendshipWithMajor(iMajor) == 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0760}}<syntaxhighlight lang="lua">local iFriendship = pPlayer:GetMinorCivFriendshipWithMajor(iActivePlayer);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0251}}<syntaxhighlight lang="lua">local iAllyInf = pPlayer:GetMinorCivFriendshipWithMajor(iAlly);</syntaxhighlight>
{{CodeLine5|0252}}<syntaxhighlight lang="lua">local iActivePlayerInf = pPlayer:GetMinorCivFriendshipWithMajor(iActivePlayer);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0059}}<syntaxhighlight lang="lua">local iInf = pMinor:GetMinorCivFriendshipWithMajor(iMajor);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0192}}<syntaxhighlight lang="lua">elseif (pMinor:GetMinorCivFriendshipWithMajor(iMajor) < GameDefines["FRIENDSHIP_THRESHOLD_NEUTRAL"]) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">local iInfluence = pMinor:GetMinorCivFriendshipWithMajor(iMajor);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0472}}<syntaxhighlight lang="lua">local info = GetStatusRow(pOtherPlayer:GetMinorCivFriendshipWithMajor(Game.GetActivePlayer()), controlTable, color);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0401}}<syntaxhighlight lang="lua">elseif (pPlayer:GetMinorCivFriendshipWithMajor(iActivePlayer) < 0) then      -- Angry</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0478}}<syntaxhighlight lang="lua">local info = GetStatusRow(pPlayer:GetMinorCivFriendshipWithMajor(iActivePlayer));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0340}}<syntaxhighlight lang="lua">pPlayer:GetMinorCivFriendshipWithMajor(iForPlayer),</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0358}}<syntaxhighlight lang="lua">pPlayer:GetMinorCivFriendshipWithMajor(iForPlayer), GameDefines["MINOR_FRIENDSHIP_AT_WAR"]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0374}}<syntaxhighlight lang="lua">elseif (pPlayer:GetMinorCivFriendshipWithMajor(iForPlayer) < 0) then      -- Angry</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0382}}<syntaxhighlight lang="lua">pPlayer:GetMinorCivFriendshipWithMajor(iForPlayer) - GameDefines["FRIENDSHIP_THRESHOLD_NEUTRAL"],</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMinorCivFriendshipWithMajor]]
[[Category:Civ5 City States API|GetMinorCivFriendshipWithMajor]]