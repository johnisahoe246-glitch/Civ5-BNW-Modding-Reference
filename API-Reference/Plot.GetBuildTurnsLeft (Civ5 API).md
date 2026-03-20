{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:GetBuildTurnsLeft<b>(</b>{{Type5|BuildActionType}} build, '''int''' nowExtra, '''int''' thenExtra<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|build:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|nowExtra:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|thenExtra:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0215}}<syntaxhighlight lang="lua">local iTurnsLeft = unit:GetPlot():GetBuildTurnsLeft(buildType, 0, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpManager.lua}}
:<code>UI/InGame/PlotHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0145}}<syntaxhighlight lang="lua">local iTurnsLeft = plot:GetBuildTurnsLeft(pBuildInfo.ID, 0, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1223}}<syntaxhighlight lang="lua">local iBuildTurns = pPlot:GetBuildTurnsLeft(iBuildID, iExtraBuildRate, iExtraBuildRate);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBuildTurnsLeft]]
[[Category:Civ5 Improvements API|GetBuildTurnsLeft]]