{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:ClearEntries<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0101}}<syntaxhighlight lang="lua">gameOption.OptionDropDown:ClearEntries();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0418}}<syntaxhighlight lang="lua">pullDown:ClearEntries();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6370}}<syntaxhighlight lang="lua">Controls.PartialMatchPullDown:ClearEntries();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0050}}<syntaxhighlight lang="lua">Controls.MultiPull:ClearEntries();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0314}}<syntaxhighlight lang="lua">Controls.ChatPull:ClearEntries();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0734}}<syntaxhighlight lang="lua">sortByPulldown:ClearEntries();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0437}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:ClearEntries();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1279}}<syntaxhighlight lang="lua">Controls.WResolutionPull:ClearEntries();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1303}}<syntaxhighlight lang="lua">Controls.FSResolutionPull:ClearEntries();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua (G&K)}}
:<code>DLC/Expansion/UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1370}}<syntaxhighlight lang="lua">Controls.TutorialPull:ClearEntries();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0434}}<syntaxhighlight lang="lua">automaticPurchasePullDown:ClearEntries();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1200}}<syntaxhighlight lang="lua">replayInfoPulldown:ClearEntries();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1216}}<syntaxhighlight lang="lua">graphDataSetPulldown:ClearEntries();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1046}}<syntaxhighlight lang="lua">cityFlagInstance.PullDown:ClearEntries();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ClearEntries]]