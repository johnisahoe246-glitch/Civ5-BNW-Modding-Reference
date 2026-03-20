{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UIManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UIManager.QueuePopup<b>(</b>{{Type5|Context}} ContextPtr, {{Type5|PopupPriority}} arg1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|ContextPtr:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 142 are listed.''

{{PseudoH4|AdvisorCounselPopup.lua}}
:<code>UI/InGame/Popups/AdvisorCounselPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0202}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.eUtmost );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0205}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.AdvisorCounsel );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorInfoPopup.lua}}
:<code>UI/InGame/Popups/AdvisorInfoPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.AdvisorInfo );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorModal.lua}}
:<code>UI/InGame/Popups/AdvisorModal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0079}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.AdvisorModal );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0033}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.CityStateDiplo );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateGreetingPopup.lua}}
:<code>UI/InGame/Popups/CityStateGreetingPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0344}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.CityStateGreeting );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0507}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.Demographics );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploOverview.lua}}
:<code>UI/InGame/Popups/DiploOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0022}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.DiploOverview );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0145}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.LeaderDiscuss );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicOverview.lua}}
:<code>UI/InGame/Popups/EconomicOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.EconOverview );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0212}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.EndGameMenu );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EULA.lua}}
:<code>UI/FrontEnd/Modding/EULA.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.ModsBrowser, PopupPriority.ModsBrowserScreen );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0063}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.LoadMenu, PopupPriority.LoadMenu );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0081}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.OptionsMenu_InGame, PopupPriority.OptionsMenu );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0041}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.AdvancedSetup, PopupPriority.AdvancedSetup );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0100}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.SelectCivilization, PopupPriority.SelectCivilization );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GoldenAgePopup.lua}}
:<code>UI/InGame/Popups/GoldenAgePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0017}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.GoldenAge );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GoodyHutPopup.lua}}
:<code>UI/InGame/Popups/GoodyHutPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0032}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.GoodyHut );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0063}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.GameMenu, PopupPriority.InGameMenu );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LeaderHeadRoot.lua}}
:<code>UI/InGame/LeaderHead/LeaderHeadRoot.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.LeaderHead );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadReplayMenu.lua}}
:<code>UI/FrontEnd/LoadReplayMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0025}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.ReplayViewer, PopupPriority.eUtmost );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MainMenu.lua}}
:<code>UI/FrontEnd/MainMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.SinglePlayerScreen, PopupPriority.SinglePlayerScreen );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.MultiplayerSelectScreen, PopupPriority.MultiplayerSelectScreen );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0094}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.Other, PopupPriority.OtherMenu );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.MilitaryOverview );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsBrowser.lua}}
:<code>UI/FrontEnd/Modding/ModsBrowser.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">UIManager:QueuePopup(Controls.ModsMenu, PopupPriority.ModsMenuScreen);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsMenu.lua}}
:<code>UI/FrontEnd/Modding/ModsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.ModdingSinglePlayer, PopupPriority.ModdingSinglePlayer );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0028}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.ModMultiplayerSelectScreen, PopupPriority.ModMultiplayerSelectScreen );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsSinglePlayer.lua}}
:<code>UI/FrontEnd/Modding/ModsSinglePlayer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">UIManager:QueuePopup(Controls.ModdingGameSetupScreen, PopupPriority.ModdingGameSetupScreen );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">UIManager:QueuePopup(Controls.LoadGameScreen, PopupPriority.LoadGameScreen );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0068}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.MPLoadGameScreen, PopupPriority.MPLoadGameScreen );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MultiplayerSelect.lua}}
:<code>UI/FrontEnd/Multiplayer/MultiplayerSelect.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.LobbyScreen, PopupPriority.LobbyScreen );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWonderPopup.lua}}
:<code>UI/InGame/Popups/NaturalWonderPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0064}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.NaturalWonderPopup );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationLogPopup.lua}}
:<code>UI/InGame/Popups/NotificationLogPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.NotificationLog );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0278}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.OptionsMenu );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OtherMenu.lua}}
:<code>UI/FrontEnd/OtherMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">UIManager:QueuePopup(Controls.Civilopedia, PopupPriority.HallOfFame);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.HallOfFame, PopupPriority.HallOfFame );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0588}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.SaveMapMenu, PopupPriority.SaveMapMenu );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCityName.lua}}
:<code>UI/InGame/Popups/SetCityName.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0126}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.Priority_GreatPersonReward );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SinglePlayer.lua}}
:<code>UI/FrontEnd/SinglePlayer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.GameSetupScreen, PopupPriority.GameSetupScreen );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0131}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.ScenariosScreen, PopupPriority.GameSetupScreen );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.LoadGameScreen, PopupPriority.LoadGameScreen );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0148}}<syntaxhighlight lang="lua">UIManager:QueuePopup( Controls.LoadTutorial, PopupPriority.LoadTutorial );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechAwardPopup.lua}}
:<code>UI/InGame/Popups/TechAwardPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0047}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.TechAward );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0515}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.TechTree );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0262}}<syntaxhighlight lang="lua">UIManager:QueuePopup( LookUpControl( "/InGame/GameMenu" ), PopupPriority.InGameMenu );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0601}}<syntaxhighlight lang="lua">UIManager:QueuePopup(Controls.VictoryStatus, PopupPriority.eUtmost);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1026}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.VictoryProgress );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0253}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.VoteResults );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WonderPopup.lua}}
:<code>UI/InGame/Popups/WonderPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">UIManager:QueuePopup( ContextPtr, PopupPriority.WonderPopup );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|QueuePopup]]