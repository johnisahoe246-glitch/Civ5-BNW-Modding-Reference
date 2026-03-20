{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.DoControl<b>(</b>{{Type5|ControlType}} control<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|control:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0145}}<syntaxhighlight lang="lua">Game.DoControl(iEndTurnControl)</syntaxhighlight>
{{CodeLine5|0146}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">Game.DoControl(GameInfoTypes.CONTROL_PREVCITY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0114}}<syntaxhighlight lang="lua">Game.DoControl(GameInfoTypes.CONTROL_NEXTCITY);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2077}}<syntaxhighlight lang="lua">Game.DoControl(GameInfoTypes.CONTROL_NEXTCITY)</syntaxhighlight>
{{CodeLine5|2078}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2084}}<syntaxhighlight lang="lua">Game.DoControl(GameInfoTypes.CONTROL_PREVCITY)</syntaxhighlight>
{{CodeLine5|2085}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0100}}<syntaxhighlight lang="lua">Game.DoControl(ControlTypes.CONTROL_RETIRE);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DoControl]]