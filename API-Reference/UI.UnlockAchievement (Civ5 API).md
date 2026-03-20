{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.UnlockAchievement<b>(</b>'''string''' arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0148}}<syntaxhighlight lang="lua">UI.UnlockAchievement("ACHIEVEMENT_SCENARIO_02_ROUTE_TO_ORIENT");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0228}}<syntaxhighlight lang="lua">UI.UnlockAchievement("ACHIEVEMENT_SCENARIO_02_RETURN_TREASURE");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0580}}<syntaxhighlight lang="lua">UI.UnlockAchievement("ACHIEVEMENT_XP1_44");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnlockAchievement]]