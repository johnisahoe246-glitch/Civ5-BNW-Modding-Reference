{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("IconSupport.lua")</code>
}}


=Usage=
<code>'''bool''' SimpleCivIconHookup<b>(</b>{{Type5|PlayerID}} player, '''int''' iconSize, {{Type5|Image}} iconControl<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|iconSize:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|iconControl:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0316}}<syntaxhighlight lang="lua">SimpleCivIconHookup(-1, 64, controlTable.Icon);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0377}}<syntaxhighlight lang="lua">SimpleCivIconHookup(-1, 64, Controls.Icon);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0469}}<syntaxhighlight lang="lua">SimpleCivIconHookup( 0, 64, Controls.IconShadow );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadScreen.lua}}
:<code>UI/FrontEnd/LoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0063}}<syntaxhighlight lang="lua">SimpleCivIconHookup( Game.GetActivePlayer(), 80, Controls.IconShadow );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0334}}<syntaxhighlight lang="lua">SimpleCivIconHookup( playerID, 64, slotInstance.Icon);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0343}}<syntaxhighlight lang="lua">SimpleCivIconHookup(-1, 64, slotInstance.Icon);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0515}}<syntaxhighlight lang="lua">SimpleCivIconHookup( Matchmaking.GetLocalID(), 64, Controls.Icon);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0479}}<syntaxhighlight lang="lua">SimpleCivIconHookup( Game.GetActivePlayer(), 64, Controls.Icon );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SimpleCivIconHookup]]