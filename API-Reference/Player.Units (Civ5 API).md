{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>iterator({{Type5|Unit}}) Player:Units<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0105}}<syntaxhighlight lang="lua">for v in player:Units() do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0418}}<syntaxhighlight lang="lua">for pUnit in pPlayer:Units() do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0420}}<syntaxhighlight lang="lua">for unit in player:Units() do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0142}}<syntaxhighlight lang="lua">for unit in pPlayer:Units()</syntaxhighlight>
{{CodeLine5|0143}}<syntaxhighlight lang="lua">   do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1082}}<syntaxhighlight lang="lua">for v in pMinorCiv:Units() do      -- for i, v in pMinorCiv:Units() do   IS IT A BUG?</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1201}}<syntaxhighlight lang="lua">for v in pMinorCiv:Units() do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1556}}<syntaxhighlight lang="lua">for w in player:Units() do</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2455}}<syntaxhighlight lang="lua">for v in pPlayer:Units() do</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Units]]
[[Category:Civ5 Units API|Units]]