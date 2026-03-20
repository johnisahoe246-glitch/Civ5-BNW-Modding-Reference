{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:GetYieldWithBuild<b>(</b>{{Type5|BuildActionType}} build, {{Type5|YieldType}} yield, '''bool''' arg2, {{Type5|PlayerID}} activePlayer<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|build:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|yield:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|activePlayer:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0267}}<syntaxhighlight lang="lua">iYieldChange = pPlot:GetYieldWithBuild(iBuild, iYield, false, Game.GetActivePlayer());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1236}}<syntaxhighlight lang="lua">iYieldChange = pPlot:GetYieldWithBuild(iBuildID, iYield, false, iActivePlayer);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetYieldWithBuild]]
[[Category:Civ5 Improvements API|GetYieldWithBuild]]
[[Category:Civ5 Yields API|GetYieldWithBuild]]