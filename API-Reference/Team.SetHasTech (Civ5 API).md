{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Team:SetHasTech<b>(</b>{{Type5|TechType}} index, '''bool''' newValue, {{Type5|PlayerID}} player, '''bool''' first, '''bool''' announce<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|index:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newValue:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|first:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|announce:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1261}}<syntaxhighlight lang="lua">pTeam:SetHasTech(iTechIndex, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetHasTech]]
[[Category:Civ5 Science API|SetHasTech]]