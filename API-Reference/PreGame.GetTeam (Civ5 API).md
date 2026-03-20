{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|TeamID}} PreGame.GetTeam<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0998}}<syntaxhighlight lang="lua">slotInstance.TeamLabel:LocalizeAndSetText( "TXT_KEY_MULTIPLAYER_DEFAULT_TEAM_NAME", PreGame.GetTeam(playerID) + 1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1000}}<syntaxhighlight lang="lua">Controls.TeamLabel:LocalizeAndSetText( "TXT_KEY_MULTIPLAYER_DEFAULT_TEAM_NAME", PreGame.GetTeam(playerID) + 1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1007}}<syntaxhighlight lang="lua">local team = PreGame.GetTeam(playerID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1025}}<syntaxhighlight lang="lua">Controls.TeamLabel:LocalizeAndSetText( "TXT_KEY_MULTIPLAYER_DEFAULT_TEAM_NAME", PreGame.GetTeam(0) + 1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1027}}<syntaxhighlight lang="lua">local team = PreGame.GetTeam(i);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1033}}<syntaxhighlight lang="lua">local playerTeam = PreGame.GetTeam(0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1037}}<syntaxhighlight lang="lua">if( PreGame.GetTeam(i) ~= playerTeam ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0223}}<syntaxhighlight lang="lua">local teamTest = PreGame.GetTeam( 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">if( PreGame.GetTeam( i ) ~= teamTest ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0363}}<syntaxhighlight lang="lua">local teamID = PreGame.GetTeam(playerID) + 1; -- Real programmers count from zero.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0528}}<syntaxhighlight lang="lua">local teamID = PreGame.GetTeam(Matchmaking.GetLocalID()) + 1; -- Real programmers count from zero.</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTeam]]
[[Category:Civ5 Diplomacy API|GetTeam]]