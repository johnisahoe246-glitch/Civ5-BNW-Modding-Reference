{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Matchmaking}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|PlayerID}} Matchmaking.GetLocalID<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0021}}<syntaxhighlight lang="lua">return Matchmaking.GetLocalID() ~= -1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0032}}<syntaxhighlight lang="lua">m_bIsInStagingRoom = (Matchmaking.GetLocalID() ~= -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">return (Matchmaking.IsHost() and PreGame.GetLoadFileName() == "") or PreGame.IsHotSeatGame() or Matchmaking.GetLocalID() == -1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0045}}<syntaxhighlight lang="lua">return (PreGame.GetLoadFileName() == "" and Matchmaking.GetLocalID() == -1) or PreGame.IsHotSeatGame();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">if(Matchmaking.GetLocalID() == -1 or Matchmaking.IsHost()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">PreGame.SetLeaderName( Matchmaking.GetLocalID(), "" );</syntaxhighlight>
{{CodeLine5|0071}}<syntaxhighlight lang="lua">PreGame.SetCivilizationDescription( Matchmaking.GetLocalID(), "" );</syntaxhighlight>
{{CodeLine5|0072}}<syntaxhighlight lang="lua">PreGame.SetCivilizationShortDescription( Matchmaking.GetLocalID(), "" );</syntaxhighlight>
{{CodeLine5|0073}}<syntaxhighlight lang="lua">PreGame.SetCivilizationAdjective( Matchmaking.GetLocalID(), "" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">local civIndex = PreGame.GetCivilization( Matchmaking.GetLocalID() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0128}}<syntaxhighlight lang="lua">return Matchmaking.GetLocalID();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0192}}<syntaxhighlight lang="lua">PreGame.SetReady( Matchmaking.GetLocalID(), bChecked );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0291}}<syntaxhighlight lang="lua">if( playerInfo.playerID == Matchmaking.GetLocalID() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0497}}<syntaxhighlight lang="lua">local playerName = playerInfo.playerName or Locale.ConvertTextKey( "TXT_KEY_MULTIPLAYER_DEFAULT_PLAYER_NAME", Matchmaking.GetLocalID() + 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0515}}<syntaxhighlight lang="lua">SimpleCivIconHookup( Matchmaking.GetLocalID(), 64, Controls.Icon);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0528}}<syntaxhighlight lang="lua">local teamID = PreGame.GetTeam(Matchmaking.GetLocalID()) + 1; -- Real programmers count from zero.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0534}}<syntaxhighlight lang="lua">Controls.HandicapLabel:LocalizeAndSetText( GameInfo.HandicapInfos( "ID = '" .. PreGame.GetHandicap( Matchmaking.GetLocalID() ) .. "'" )().Description );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0540}}<syntaxhighlight lang="lua">local bIsReady = PreGame.IsReady( Matchmaking.GetLocalID() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0543}}<syntaxhighlight lang="lua">PreGame.SetReady(Matchmaking.GetLocalID(), true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0564}}<syntaxhighlight lang="lua">Controls.HostIcon:SetHide( Matchmaking.GetLocalID() ~= m_HostID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0743}}<syntaxhighlight lang="lua">if( playerID ~= Matchmaking.GetLocalID() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0856}}<syntaxhighlight lang="lua">PreGame.SetReady( Matchmaking.GetLocalID() );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetLocalID]]