{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>{{Type5|ResourceType}}, {{Type5|PlayerID}} ToGridFromHex<b>(</b>'''float''' i, '''float''' j<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|i:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|j:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0592}}<syntaxhighlight lang="lua">local gridPosX, gridPosY = ToGridFromHex( hexPos.x, hexPos.y );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0664}}<syntaxhighlight lang="lua">local gridPosX, gridPosY = ToGridFromHex( instance.Hex.x, instance.Hex.y );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0969}}<syntaxhighlight lang="lua">local gridX, gridY = ToGridFromHex( i, j );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceIconManager.lua}}
:<code>UI/InGame/ResourceIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">local gridX, gridY  = ToGridFromHex( hexPosX, hexPosY );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2414}}<syntaxhighlight lang="lua">local iX, iY = ToGridFromHex(i, j);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2704}}<syntaxhighlight lang="lua">local iX, iY = ToGridFromHex( HPosX, HPosY );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1252}}<syntaxhighlight lang="lua">local gridVecX, gridVecY = ToGridFromHex( hexPos.x, hexPos.y );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1441}}<syntaxhighlight lang="lua">local pPlot = Map.GetPlot( ToGridFromHex( hexPos.x, hexPos.y ) );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ToGridFromHex]]