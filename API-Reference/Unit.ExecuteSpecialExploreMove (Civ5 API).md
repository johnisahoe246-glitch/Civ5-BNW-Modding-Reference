{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Unit:ExecuteSpecialExploreMove<b>(</b>{{Type5|Plot}} targetPlot<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|targetPlot:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0569}}<syntaxhighlight lang="lua">pUnit:ExecuteSpecialExploreMove(pTargetPlot);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ExecuteSpecialExploreMove]]
[[Category:Civ5 Units API|ExecuteSpecialExploreMove]]
[[Category:Civ5 Movement API|ExecuteSpecialExploreMove]]