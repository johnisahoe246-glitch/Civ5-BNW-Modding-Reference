{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:BuildEntry<b>(</b>'''string''' arg0, '''table''' arg1<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">gameOption.OptionDropDown:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0421}}<syntaxhighlight lang="lua">pullDown:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0481}}<syntaxhighlight lang="lua">pullDown:BuildEntry( "InstanceOne", instance );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6374}}<syntaxhighlight lang="lua">Controls.PartialMatchPullDown:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">Controls.MultiPull:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0319}}<syntaxhighlight lang="lua">Controls.ChatPull:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoCorner.lua}}
:<code>UI/InGame/InfoCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0105}}<syntaxhighlight lang="lua">Controls.LeftPull:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0737}}<syntaxhighlight lang="lua">sortByPulldown:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0417}}<syntaxhighlight lang="lua">Controls.GameSpeedPullDown:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0441}}<syntaxhighlight lang="lua">Controls.MapSizePullDown:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0714}}<syntaxhighlight lang="lua">Controls.EraPull:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1154}}<syntaxhighlight lang="lua">pulldown:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1176}}<syntaxhighlight lang="lua">Controls.LeaderPull:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1198}}<syntaxhighlight lang="lua">Controls.MSAAPull:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1288}}<syntaxhighlight lang="lua">Controls.WResolutionPull:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1321}}<syntaxhighlight lang="lua">Controls.FSResolutionPull:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0410}}<syntaxhighlight lang="lua">automaticPurchasePullDown:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1203}}<syntaxhighlight lang="lua">replayInfoPulldown:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1227}}<syntaxhighlight lang="lua">graphDataSetPulldown:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UITestMenu.lua}}
:<code>UI/FrontEnd/UITestMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">Controls.PullDown:BuildEntry( "InstanceOne", controlTable );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0119}}<syntaxhighlight lang="lua">Controls.PullDown:BuildEntry( "InstanceTwo", controlTable );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1054}}<syntaxhighlight lang="lua">cityFlagInstance.PullDown:BuildEntry( "UnitInstance", controlTable );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|BuildEntry]]
[[Category:Civ5 Improvements API|BuildEntry]]