{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Grid}} and {{Type5|Image}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:DoAutoSize<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0036}}<syntaxhighlight lang="lua">Controls.Grid:DoAutoSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0554}}<syntaxhighlight lang="lua">Controls.DetailsGrid:DoAutoSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0185}}<syntaxhighlight lang="lua">Controls.OptionsPanel:DoAutoSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0246}}<syntaxhighlight lang="lua">Controls.LegendFrame:DoAutoSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpText.lua}}
:<code>UI/InGame/WorldView/PlotHelpText.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0072}}<syntaxhighlight lang="lua">Controls.TextBox:DoAutoSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TaskList.lua}}
:<code>UI/InGame/TaskList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0043}}<syntaxhighlight lang="lua">Controls.TaskListGrid:DoAutoSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechAwardPopup.lua}}
:<code>UI/InGame/Popups/TechAwardPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0083}}<syntaxhighlight lang="lua">Controls.OuterGrid:DoAutoSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0582}}<syntaxhighlight lang="lua">Controls.MainGrid:DoAutoSize();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DoAutoSize]]