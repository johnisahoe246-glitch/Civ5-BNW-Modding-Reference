{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetGoldPerTurnFromDiplomacy<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">local diploGPT = pPlayer:GetGoldPerTurnFromDiplomacy();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0362}}<syntaxhighlight lang="lua">Controls.DiploExpenseValue:SetText( Locale.ToNumber( pPlayer:GetGoldPerTurnFromDiplomacy(), "#.##" ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0423}}<syntaxhighlight lang="lua">local iGoldPerTurnFromOtherPlayers = pPlayer:GetGoldPerTurnFromDiplomacy();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetGoldPerTurnFromDiplomacy]]
[[Category:Civ5 Gold API|GetGoldPerTurnFromDiplomacy]]
[[Category:Civ5 Diplomacy API|GetGoldPerTurnFromDiplomacy]]