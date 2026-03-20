{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetGold<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|BarbarianRansomPopup.lua}}
:<code>UI/InGame/PopupsGeneric/BarbarianRansomPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0011}}<syntaxhighlight lang="lua">if (iNumGold > pPlayer:GetGold()) then</syntaxhighlight>
{{CodeLine5|0012}}<syntaxhighlight lang="lua">iNumGold = pPlayer:GetGold();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0725}}<syntaxhighlight lang="lua">local iNumGoldPlayerHas = pActivePlayer:GetGold();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0181}}<syntaxhighlight lang="lua">Controls.TotalGoldValue:SetText( Locale.ToNumber( pPlayer:GetGold(), "#.##" ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0045}}<syntaxhighlight lang="lua">if (pPlayer:GetGold() + iGoldPerTurn < 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">local iTotalGold = pPlayer:GetGold();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1276}}<syntaxhighlight lang="lua">if (Players[g_iUs]:GetGold() < iCost or Players[g_iThem]:GetGold() < iCost or bEmptyTT) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1886}}<syntaxhighlight lang="lua">if (player:GetGold() >= 400) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2858}}<syntaxhighlight lang="lua">if (pPlayer:GetGold() < 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0970}}<syntaxhighlight lang="lua">if (iGoldToUpgrade > pActivePlayer:GetGold()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WhosWinningPopup.lua}}
:<code>UI/InGame/Popups/WhosWinningPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0224}}<syntaxhighlight lang="lua">return pPlayer:GetGold();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGold]]
[[Category:Civ5 Gold API|GetGold]]