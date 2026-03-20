{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:AssignCityStatesToRegionsOrToUninhabited<b>(</b>'''unknown''' args<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|args:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6653}}<syntaxhighlight lang="lua">self:AssignCityStatesToRegionsOrToUninhabited()</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6655}}<syntaxhighlight lang="lua">--print("-"); print("--- City State Placement Results ---");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6657}}<syntaxhighlight lang="lua">local iW, iH = Map.GetGridSize();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AssignCityStatesToRegionsOrToUninhabited]]
[[Category:Civ5 Cities API|AssignCityStatesToRegionsOrToUninhabited]]