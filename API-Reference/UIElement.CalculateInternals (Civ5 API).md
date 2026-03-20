{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:CalculateInternals<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0148}}<syntaxhighlight lang="lua">gameOption.OptionDropDown:CalculateInternals();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0435}}<syntaxhighlight lang="lua">pullDown:CalculateInternals();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6385}}<syntaxhighlight lang="lua">Controls.PartialMatchPullDown:CalculateInternals();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0071}}<syntaxhighlight lang="lua">Controls.MultiPull:CalculateInternals();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0361}}<syntaxhighlight lang="lua">Controls.ChatPull:CalculateInternals();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoCorner.lua}}
:<code>UI/InGame/InfoCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0121}}<syntaxhighlight lang="lua">Controls.LeftPull:CalculateInternals();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0748}}<syntaxhighlight lang="lua">sortByPulldown:CalculateInternals();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0423}}<syntaxhighlight lang="lua">Controls.GameSpeedPullDown:CalculateInternals();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0454}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:CalculateInternals();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0718}}<syntaxhighlight lang="lua">Controls.EraPull:CalculateInternals();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1158}}<syntaxhighlight lang="lua">pulldown:CalculateInternals();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1188}}<syntaxhighlight lang="lua">Controls.LeaderPull:CalculateInternals();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1206}}<syntaxhighlight lang="lua">Controls.MSAAPull:CalculateInternals();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1295}}<syntaxhighlight lang="lua">Controls.WResolutionPull:CalculateInternals();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1328}}<syntaxhighlight lang="lua">Controls.FSResolutionPull:CalculateInternals();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0467}}<syntaxhighlight lang="lua">automaticPurchasePullDown:CalculateInternals();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1211}}<syntaxhighlight lang="lua">replayInfoPulldown:CalculateInternals();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1234}}<syntaxhighlight lang="lua">graphDataSetPulldown:CalculateInternals();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UITestMenu.lua}}
:<code>UI/FrontEnd/UITestMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0126}}<syntaxhighlight lang="lua">Controls.PullDown:CalculateInternals();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1081}}<syntaxhighlight lang="lua">cityFlagInstance.PullDown:CalculateInternals();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CalculateInternals]]