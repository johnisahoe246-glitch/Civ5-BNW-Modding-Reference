{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' City:SetNumRealBuilding<b>(</b>{{Type5|BuildingType}} index, '''int''' newValue<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|index:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newValue:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0972}}<syntaxhighlight lang="lua">pCity:SetNumRealBuilding(GameInfoTypes["BUILDING_MONUMENT"], 1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0827}}<syntaxhighlight lang="lua">pVaticanCity:SetNumRealBuilding(iBuildingID, 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1084}}<syntaxhighlight lang="lua">capital:SetNumRealBuilding(iBuildingID, 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1130}}<syntaxhighlight lang="lua">cityState:SetNumRealBuilding(iBuildingID, 1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetNumRealBuilding]]
[[Category:Civ5 Buildings API|SetNumRealBuilding]]