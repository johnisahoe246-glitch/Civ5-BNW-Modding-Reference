{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Map.GetCustomOption<b>(</b>'''int''' optionIndex<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|optionIndex:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 133 are listed.''

{{PseudoH4|Arborea.lua (G&K)}}
:<code>DLC/Expansion/Maps/Arborea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0113}}<syntaxhighlight lang="lua">local sea_level = Map.GetCustomOption(4)</syntaxhighlight>
{{CodeLine5|0114}}<syntaxhighlight lang="lua">if sea_level == 4 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">local world_age = Map.GetCustomOption(1)</syntaxhighlight>
{{CodeLine5|0118}}<syntaxhighlight lang="lua">if world_age == 4 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0631}}<syntaxhighlight lang="lua">userInputLandmass = Map.GetCustomOption(6) -- GLOBAL variable</syntaxhighlight>
{{CodeLine5|0632}}<syntaxhighlight lang="lua">if userInputLandmass == 5 then -- Random</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0673}}<syntaxhighlight lang="lua">local sea = Map.GetCustomOption(4)</syntaxhighlight>
{{CodeLine5|0674}}<syntaxhighlight lang="lua">if sea == 4 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0677}}<syntaxhighlight lang="lua">local age = Map.GetCustomOption(1)</syntaxhighlight>
{{CodeLine5|0678}}<syntaxhighlight lang="lua">if age == 4 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0719}}<syntaxhighlight lang="lua">local temp = Map.GetCustomOption(2)</syntaxhighlight>
{{CodeLine5|0720}}<syntaxhighlight lang="lua">if temp == 4 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0743}}<syntaxhighlight lang="lua">local rain = Map.GetCustomOption(3)</syntaxhighlight>
{{CodeLine5|0744}}<syntaxhighlight lang="lua">if rain == 4 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0907}}<syntaxhighlight lang="lua">local res = Map.GetCustomOption(5)</syntaxhighlight>
{{CodeLine5|0908}}<syntaxhighlight lang="lua">if res == 6 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0593}}<syntaxhighlight lang="lua">local rain = Map.GetCustomOption(2)</syntaxhighlight>
{{CodeLine5|0594}}<syntaxhighlight lang="lua">if rain == 4 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0776}}<syntaxhighlight lang="lua">local res = Map.GetCustomOption(3)</syntaxhighlight>
{{CodeLine5|0777}}<syntaxhighlight lang="lua">if res == 6 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Four_Corners.lua}}
:<code>Maps/Four_Corners.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0121}}<syntaxhighlight lang="lua">local buffer_setting = Map.GetCustomOption(5)</syntaxhighlight>
{{CodeLine5|0122}}<syntaxhighlight lang="lua">if buffer_setting == 3 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0530}}<syntaxhighlight lang="lua">local res = Map.GetCustomOption(4)</syntaxhighlight>
{{CodeLine5|0531}}<syntaxhighlight lang="lua">if res == 6 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Frontier.lua (G&K)}}
:<code>DLC/Expansion/Maps/Frontier.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0627}}<syntaxhighlight lang="lua">userInputLandmass = Map.GetCustomOption(6)</syntaxhighlight>
{{CodeLine5|0628}}<syntaxhighlight lang="lua">if userInputLandmass == 3 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Hemispheres.lua (G&K)}}
:<code>DLC/Expansion/Maps/Hemispheres.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0170}}<syntaxhighlight lang="lua">local island_setting = Map.GetCustomOption(5)</syntaxhighlight>
{{CodeLine5|0171}}<syntaxhighlight lang="lua">if island_setting == 5 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0940}}<syntaxhighlight lang="lua">local team_setting = Map.GetCustomOption(6)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0942}}<syntaxhighlight lang="lua">-- If two teams are present, use team-oriented handling of start points, one team west, one east.</syntaxhighlight>
{{CodeLine5|0943}}<syntaxhighlight lang="lua">if iNumTeams == 2 and team_setting == 1 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1120}}<syntaxhighlight lang="lua">local team_setting = Map.GetCustomOption(5)</syntaxhighlight>
{{CodeLine5|1121}}<syntaxhighlight lang="lua">if iNumTeams == 2 and team_setting == 1 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Highlands.lua}}
:<code>Maps/Highlands.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">local userInputGrain = Map.GetCustomOption(4)</syntaxhighlight>
{{CodeLine5|0118}}<syntaxhighlight lang="lua">local userInputPeaks = Map.GetCustomOption(5)</syntaxhighlight>
{{CodeLine5|0119}}<syntaxhighlight lang="lua">local userInputLakes = Map.GetCustomOption(6)</syntaxhighlight>
{{CodeLine5|0120}}<syntaxhighlight lang="lua">if userInputGrain == 5 then -- Random</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0231}}<syntaxhighlight lang="lua">local temp = Map.GetCustomOption(1)</syntaxhighlight>
{{CodeLine5|0232}}<syntaxhighlight lang="lua">if temp == 4 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ice_Age.lua}}
:<code>Maps/Ice_Age.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0102}}<syntaxhighlight lang="lua">local userInputLandmass = Map.GetCustomOption(6)</syntaxhighlight>
{{CodeLine5|0103}}<syntaxhighlight lang="lua">land_type = userInputLandmass - 1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0235}}<syntaxhighlight lang="lua">local temperature = Map.GetCustomOption(2)</syntaxhighlight>
{{CodeLine5|0236}}<syntaxhighlight lang="lua">if temperature == 4 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lakes.lua}}
:<code>Maps/Lakes.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">local userInputLakes = Map.GetCustomOption(5)</syntaxhighlight>
{{CodeLine5|0090}}<syntaxhighlight lang="lua">if userInputLakes == 4 then -- Random</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|North_vs_South.lua}}
:<code>Maps/North_vs_South.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0491}}<syntaxhighlight lang="lua">local team_setting = Map.GetCustomOption(5)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0493}}<syntaxhighlight lang="lua">-- If two teams are present, use team-oriented handling of start points, one team north, one south.</syntaxhighlight>
{{CodeLine5|0494}}<syntaxhighlight lang="lua">if iNumTeams == 2 and team_setting == 1 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ring.lua}}
:<code>Maps/Ring.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0130}}<syntaxhighlight lang="lua">dominant_terrain = Map.GetCustomOption(1) -- GLOBAL variable.</syntaxhighlight>
{{CodeLine5|0131}}<syntaxhighlight lang="lua">if dominant_terrain == 5 then -- Random</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0134}}<syntaxhighlight lang="lua">local landmass_type = Map.GetCustomOption(2);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0138}}<syntaxhighlight lang="lua">local bridge_width = Map.GetCustomOption(3)</syntaxhighlight>
{{CodeLine5|0139}}<syntaxhighlight lang="lua">if bridge_width == 4 then -- Random</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">dominant_terrain = Map.GetCustomOption(1) -- GLOBAL variable.</syntaxhighlight>
{{CodeLine5|0105}}<syntaxhighlight lang="lua">if dominant_terrain == 9 then -- Random</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0108}}<syntaxhighlight lang="lua">userInputWaterSetting = Map.GetCustomOption(2) -- GLOBAL variable.</syntaxhighlight>
{{CodeLine5|0109}}<syntaxhighlight lang="lua">if userInputWaterSetting == 6 then -- Random</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Tilted_Axis.lua (G&K)}}
:<code>DLC/Expansion/Maps/Tilted_Axis.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0134}}<syntaxhighlight lang="lua">local sea_level = Map.GetCustomOption(3)</syntaxhighlight>
{{CodeLine5|0135}}<syntaxhighlight lang="lua">if sea_level == 3 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0648}}<syntaxhighlight lang="lua">userInputLandmass = Map.GetCustomOption(5) -- GLOBAL variable</syntaxhighlight>
{{CodeLine5|0649}}<syntaxhighlight lang="lua">if userInputLandmass == 5 then -- Random</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0690}}<syntaxhighlight lang="lua">local sea = Map.GetCustomOption(3)</syntaxhighlight>
{{CodeLine5|0691}}<syntaxhighlight lang="lua">if sea == 3 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|West_vs_East.lua}}
:<code>Maps/West_vs_East.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0313}}<syntaxhighlight lang="lua">local team_setting = Map.GetCustomOption(5)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0315}}<syntaxhighlight lang="lua">-- If two teams are present, use team-oriented handling of start points, one team west, one east.</syntaxhighlight>
{{CodeLine5|0316}}<syntaxhighlight lang="lua">if iNumTeams == 2 and team_setting == 1 then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCustomOption]]
[[Category:Civ5 Game Settings API|GetCustomOption]]