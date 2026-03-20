{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Plot:IsFriendlyTerritory<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0824}}<syntaxhighlight lang="lua">if (pToPlot:IsFriendlyTerritory(iMyPlayer)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0844}}<syntaxhighlight lang="lua">if (not pToPlot:IsFriendlyTerritory(iMyPlayer)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1202}}<syntaxhighlight lang="lua">if (pToPlot:IsFriendlyTerritory(iTheirPlayer)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1212}}<syntaxhighlight lang="lua">if (not pToPlot:IsFriendlyTerritory(iTheirPlayer)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1530}}<syntaxhighlight lang="lua">if (theirPlot:IsFriendlyTerritory(iTheirPlayer)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1540}}<syntaxhighlight lang="lua">if (not theirPlot:IsFriendlyTerritory(iTheirPlayer)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0877}}<syntaxhighlight lang="lua">if (pToPlot:IsFriendlyTerritory(c)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsFriendlyTerritory]]
[[Category:Civ5 Movement API|IsFriendlyTerritory]]