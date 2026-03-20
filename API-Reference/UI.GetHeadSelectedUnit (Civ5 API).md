{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|Unit}} UI.GetHeadSelectedUnit<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1791}}<syntaxhighlight lang="lua">local pHeadUnit = UI.GetHeadSelectedUnit();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0234}}<syntaxhighlight lang="lua">local pUnit = UI.GetHeadSelectedUnit();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0433}}<syntaxhighlight lang="lua">local unit = UI.GetHeadSelectedUnit();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0529}}<syntaxhighlight lang="lua">local pHeadSelectedUnit = UI.GetHeadSelectedUnit();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0068}}<syntaxhighlight lang="lua">local pSelectedUnit = UI:GetHeadSelectedUnit();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0822}}<syntaxhighlight lang="lua">if UI.GetHeadSelectedUnit() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0825}}<syntaxhighlight lang="lua">Data1 = UI.GetHeadSelectedUnit():GetID(),</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHeadSelectedUnit]]
[[Category:Civ5 Units API|GetHeadSelectedUnit]]