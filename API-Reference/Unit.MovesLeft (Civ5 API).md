{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:MovesLeft<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0164}}<syntaxhighlight lang="lua">if( unit:MovesLeft() > 0 ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0235}}<syntaxhighlight lang="lua">local moves_left = math.floor(unit:MovesLeft() / move_denominator);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">if (v:IsFound() and v:MovesLeft() > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0561}}<syntaxhighlight lang="lua">if (v:IsHurt() and v:CanHeal(plot) and v:MovesLeft() > 0 and v:IsSelected()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0586}}<syntaxhighlight lang="lua">if (v:IsHurt() and v:CanHeal(plot) and v:MovesLeft() > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1502}}<syntaxhighlight lang="lua">if (v:IsFound() and  v:MovesLeft() > 0 and v:IsSelected()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1552}}<syntaxhighlight lang="lua">if (v:MovesLeft() > 0 and v:IsSelected()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1555}}<syntaxhighlight lang="lua">local iMovesLeft = v:MovesLeft() / move_denominator;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0697}}<syntaxhighlight lang="lua">if( pUnit:MovesLeft() > 0 ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1071}}<syntaxhighlight lang="lua">if( pPlotUnit:MovesLeft() > 0 ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0215}}<syntaxhighlight lang="lua">local moves_left = unit:MovesLeft() / move_denominator;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0143}}<syntaxhighlight lang="lua">local bUnitHasMovesLeft = unit:MovesLeft() > 0;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|MovesLeft]]
[[Category:Civ5 Movement API|MovesLeft]]