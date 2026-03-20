{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|HandicapType}} PreGame.GetHandicap<b>(</b>{{Type5|PlayerID}} player = nil<b>)</b></code>


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
{{CodeLine5|0572}}<syntaxhighlight lang="lua">local info = GameInfo.HandicapInfos[PreGame.GetHandicap(0)];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">local iHandicap = PreGame.GetHandicap(0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0373}}<syntaxhighlight lang="lua">info = GameInfo.HandicapInfos[ PreGame.GetHandicap( 0 ) ];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0312}}<syntaxhighlight lang="lua">local info = GameInfo.HandicapInfos[ PreGame.GetHandicap( 0 ) ];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0072}}<syntaxhighlight lang="lua">PreGame.GetHandicap(), PreGame.GetWorldSize(), PreGame.GetMapScript(), nil,</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0369}}<syntaxhighlight lang="lua">slotInstance.HandicapLabel:LocalizeAndSetText( GameInfo.HandicapInfos( "ID = '" .. PreGame.GetHandicap( playerID ) .. "'" )().Description );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0534}}<syntaxhighlight lang="lua">Controls.HandicapLabel:LocalizeAndSetText( GameInfo.HandicapInfos( "ID = '" .. PreGame.GetHandicap( Matchmaking.GetLocalID() ) .. "'" )().Description );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHandicap]]
[[Category:Civ5 Game Settings API|GetHandicap]]