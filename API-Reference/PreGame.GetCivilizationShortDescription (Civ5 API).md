{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''string''' PreGame.GetCivilizationShortDescription<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


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
{{CodeLine5|0343}}<syntaxhighlight lang="lua">local civName = PreGame.GetCivilizationShortDescription(0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0230}}<syntaxhighlight lang="lua">if(PreGame.GetCivilizationShortDescription(g_iPlayer) ~= "") then</syntaxhighlight>
{{CodeLine5|0231}}<syntaxhighlight lang="lua">TruncateString(Controls.CivName, textBoxSize, Locale.ConvertTextKey(PreGame.GetCivilizationShortDescription(g_iPlayer)));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0210}}<syntaxhighlight lang="lua">elseif( iPlayer == Game.GetActivePlayer() and PreGame.GetCivilizationShortDescription( 0 ) ~= "" ) then</syntaxhighlight>
{{CodeLine5|0211}}<syntaxhighlight lang="lua">Controls.CivIconFrame:SetToolTipString( PreGame.GetCivilizationShortDescription( 0 ) .. "     " .. Locale.ConvertTextKey( gameTrait.ShortDescription ) .. "[NEWLINE]" .. Locale.ConvertTextKey( gameTrait.Description ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0327}}<syntaxhighlight lang="lua">elseif(iPlayer == Game.GetActivePlayer() and PreGame.GetCivilizationShortDescription(0) ~= "") then</syntaxhighlight>
{{CodeLine5|0328}}<syntaxhighlight lang="lua">TruncateString(Controls.DetailsCiv, availableTextExtent, PreGame.GetCivilizationShortDescription(0));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameplayUtilities.lua}}
:<code>Gameplay/Lua/GameplayUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0033}}<syntaxhighlight lang="lua">local civShortDescription = PreGame.GetCivilizationShortDescription(playerID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0225}}<syntaxhighlight lang="lua">name = PreGame.GetCivilizationShortDescription(g_EditSlot);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0385}}<syntaxhighlight lang="lua">if(PreGame.GetCivilizationShortDescription(pPlayer:GetID()) ~= "") then</syntaxhighlight>
{{CodeLine5|0386}}<syntaxhighlight lang="lua">strPlayer = PreGame.GetCivilizationShortDescription(pPlayer:GetID());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0865}}<syntaxhighlight lang="lua">strCiv = PreGame.GetCivilizationShortDescription(pPlayer:GetID());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCivilizationShortDescription]]
[[Category:Civ5 Players API|GetCivilizationShortDescription]]