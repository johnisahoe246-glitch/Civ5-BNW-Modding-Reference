{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' City:SetPopulation<b>(</b>'''int''' newValue, '''bool''' flag<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|newValue:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|flag:
|valign="top"| ''Must be true to allow new citizens to work on tiles.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1071}}<syntaxhighlight lang="lua">capital:SetPopulation(5, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1126}}<syntaxhighlight lang="lua">cityState:SetPopulation(3, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetPopulation]]
[[Category:Civ5 Food & Population API|SetPopulation]]