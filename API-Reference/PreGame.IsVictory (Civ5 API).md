{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' PreGame.IsVictory<b>(</b>'''string''' arg0<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1060}}<syntaxhighlight lang="lua">victoryCondition.GameOptionRoot:SetCheck(PreGame.IsVictory(row.Type));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0396}}<syntaxhighlight lang="lua">if(PreGame.IsVictory(row.ID) == true) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0882}}<syntaxhighlight lang="lua">victoryCondition.GameOptionRoot:SetCheck(PreGame.IsVictory(row.ID));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0177}}<syntaxhighlight lang="lua">if(PreGame.IsVictory(GameInfo.Victories["VICTORY_TIME"].ID))then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0284}}<syntaxhighlight lang="lua">if(PreGame.IsVictory(GameInfo.Victories["VICTORY_SPACE_RACE"].ID))then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0358}}<syntaxhighlight lang="lua">if(PreGame.IsVictory(GameInfo.Victories["VICTORY_DIPLOMATIC"].ID))then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0433}}<syntaxhighlight lang="lua">if(PreGame.IsVictory(GameInfo.Victories["VICTORY_CULTURAL"].ID))then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsVictory]]
[[Category:Civ5 Victory API|IsVictory]]