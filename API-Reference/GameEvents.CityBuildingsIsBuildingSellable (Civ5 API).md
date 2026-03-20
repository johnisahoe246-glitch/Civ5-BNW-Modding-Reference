{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
<br/>
*This method was added in Gods & Kings.
}}


=Usage=
<code>'''void''' GameEvents.CityBuildingsIsBuildingSellable<b>(</b>{{Type5|PlayerID}} player, {{Type5|BuildingType}} building<b>)</b></code>


'''Event Type'''
:Unknown

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|building:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0483}}<syntaxhighlight lang="lua">GameEvents.CityBuildingsIsBuildingSellable.Add(IsBuildingSellable);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CityBuildingsIsBuildingSellable]]
[[Category:Civ5 Cities API|CityBuildingsIsBuildingSellable]]
[[Category:Civ5 Buildings API|CityBuildingsIsBuildingSellable]]