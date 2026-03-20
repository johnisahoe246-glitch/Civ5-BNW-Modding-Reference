{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''', '''bool''' AssignStartingPlots:FindCoastalStart<b>(</b>'''int''' region_number<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|region_number:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|3434}}<syntaxhighlight lang="lua">bSuccessFlag, bForcedPlacementFlag = self:FindCoastalStart(currentRegionNumber)</syntaxhighlight>
{{CodeLine5|3435}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|FindCoastalStart]]
[[Category:Civ5 Terrain API|FindCoastalStart]]