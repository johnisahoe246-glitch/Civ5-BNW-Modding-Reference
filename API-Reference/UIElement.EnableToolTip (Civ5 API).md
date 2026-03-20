{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:EnableToolTip<b>(</b>'''bool''' arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1205}}<syntaxhighlight lang="lua">cityBanner.SubControls.BannerButton:EnableToolTip(not disableBanners);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0751}}<syntaxhighlight lang="lua">controlTable.CivVotes:EnableToolTip(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0754}}<syntaxhighlight lang="lua">controlTable.CivVotes:EnableToolTip(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0761}}<syntaxhighlight lang="lua">controlTable.MinorVotes:EnableToolTip(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0764}}<syntaxhighlight lang="lua">controlTable.MinorVotes:EnableToolTip(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0771}}<syntaxhighlight lang="lua">controlTable.LiberatedCSVotes:EnableToolTip(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0774}}<syntaxhighlight lang="lua">controlTable.LiberatedCSVotes:EnableToolTip(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0792}}<syntaxhighlight lang="lua">controlTable.LastVoteCivIcon:EnableToolTip(false);</syntaxhighlight>
{{CodeLine5|0793}}<syntaxhighlight lang="lua">controlTable.LastVoteCivIconBG:EnableToolTip(false);</syntaxhighlight>
{{CodeLine5|0794}}<syntaxhighlight lang="lua">controlTable.LastVoteCivIconShadow:EnableToolTip(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0818}}<syntaxhighlight lang="lua">controlTable.LastVoteCivIcon:EnableToolTip(true);</syntaxhighlight>
{{CodeLine5|0819}}<syntaxhighlight lang="lua">controlTable.LastVoteCivIconBG:EnableToolTip(true);</syntaxhighlight>
{{CodeLine5|0820}}<syntaxhighlight lang="lua">controlTable.LastVoteCivIconShadow:EnableToolTip(true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0831}}<syntaxhighlight lang="lua">controlTable.ProjectedVotes:EnableToolTip(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0843}}<syntaxhighlight lang="lua">controlTable.ProjectedVotes:EnableToolTip(true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0200}}<syntaxhighlight lang="lua">controlTable.VoteCastBox:EnableToolTip(false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0202}}<syntaxhighlight lang="lua">controlTable.VoteCastBox:EnableToolTip(true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|EnableToolTip]]