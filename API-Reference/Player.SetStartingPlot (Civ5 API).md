{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Player:SetStartingPlot<b>(</b>{{Type5|Plot}} plot<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|plot:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 68 are listed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|4597}}<syntaxhighlight lang="lua">player:SetStartingPlot(start_plot)</syntaxhighlight>
{{CodeLine5|4598}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4737}}<syntaxhighlight lang="lua">player:SetStartingPlot(plot);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6630}}<syntaxhighlight lang="lua">cityState:SetStartingPlot(cs_start_plot)</syntaxhighlight>
{{CodeLine5|6631}}<syntaxhighlight lang="lua">self:GenerateLuxuryPlotListsAtCitySite(x, y, 1, true) -- Removes Feature Ice from coasts adjacent to the city state's new location</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6745}}<syntaxhighlight lang="lua">cityState:SetStartingPlot(cs_start_plot)</syntaxhighlight>
{{CodeLine5|6746}}<syntaxhighlight lang="lua">self:GenerateLuxuryPlotListsAtCitySite(cs_x, cs_y, 1, true) -- Removes Feature Ice from coasts adjacent to the city state's new location</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe_Scenario.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/Europe_Scenario.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1208}}<syntaxhighlight lang="lua">player:SetStartingPlot(start_plot)</syntaxhighlight>
{{CodeLine5|1209}}<syntaxhighlight lang="lua">--print("England being placed in plot " .. x .. ", " .. y .. ".");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1211}}<syntaxhighlight lang="lua">-- Celts</syntaxhighlight>
{{CodeLine5|1212}}<syntaxhighlight lang="lua">local region_number = 1;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1217}}<syntaxhighlight lang="lua">player:SetStartingPlot(start_plot)</syntaxhighlight>
{{CodeLine5|1218}}<syntaxhighlight lang="lua">--print("Celts being placed in plot " .. x .. ", " .. y .. ".");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1220}}<syntaxhighlight lang="lua">-- Arabia</syntaxhighlight>
{{CodeLine5|1221}}<syntaxhighlight lang="lua">local region_number = 3;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1226}}<syntaxhighlight lang="lua">player:SetStartingPlot(start_plot)</syntaxhighlight>
{{CodeLine5|1227}}<syntaxhighlight lang="lua">--print("Arabia being placed in plot " .. x .. ", " .. y .. ".");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1229}}<syntaxhighlight lang="lua">-- Songhai</syntaxhighlight>
{{CodeLine5|1230}}<syntaxhighlight lang="lua">local region_number = 4;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1235}}<syntaxhighlight lang="lua">player:SetStartingPlot(start_plot)</syntaxhighlight>
{{CodeLine5|1236}}<syntaxhighlight lang="lua">--print("Songhai being placed in plot " .. x .. ", " .. y .. ".");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1238}}<syntaxhighlight lang="lua">-- Ottomans</syntaxhighlight>
{{CodeLine5|1239}}<syntaxhighlight lang="lua">local region_number = 5;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1244}}<syntaxhighlight lang="lua">player:SetStartingPlot(start_plot)</syntaxhighlight>
{{CodeLine5|1245}}<syntaxhighlight lang="lua">--print("Ottomans being placed in plot " .. x .. ", " .. y .. ".");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1247}}<syntaxhighlight lang="lua">-- Byzantium</syntaxhighlight>
{{CodeLine5|1248}}<syntaxhighlight lang="lua">local region_number = 6;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1253}}<syntaxhighlight lang="lua">player:SetStartingPlot(start_plot)</syntaxhighlight>
{{CodeLine5|1254}}<syntaxhighlight lang="lua">--print("Byzantium being placed in plot " .. x .. ", " .. y .. ".");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1256}}<syntaxhighlight lang="lua">-- Spain</syntaxhighlight>
{{CodeLine5|1257}}<syntaxhighlight lang="lua">local region_number = 7;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1262}}<syntaxhighlight lang="lua">player:SetStartingPlot(start_plot)</syntaxhighlight>
{{CodeLine5|1263}}<syntaxhighlight lang="lua">--print("Spain being placed in plot " .. x .. ", " .. y .. ".");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1265}}<syntaxhighlight lang="lua">-- France</syntaxhighlight>
{{CodeLine5|1266}}<syntaxhighlight lang="lua">local region_number = 8;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1271}}<syntaxhighlight lang="lua">player:SetStartingPlot(start_plot)</syntaxhighlight>
{{CodeLine5|1272}}<syntaxhighlight lang="lua">--print("France being placed in plot " .. x .. ", " .. y .. ".");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1274}}<syntaxhighlight lang="lua">-- Netherlands</syntaxhighlight>
{{CodeLine5|1275}}<syntaxhighlight lang="lua">local region_number = 9;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1280}}<syntaxhighlight lang="lua">player:SetStartingPlot(start_plot)</syntaxhighlight>
{{CodeLine5|1281}}<syntaxhighlight lang="lua">--print("Netherlands being placed in plot " .. x .. ", " .. y .. ".");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1283}}<syntaxhighlight lang="lua">-- Austria</syntaxhighlight>
{{CodeLine5|1284}}<syntaxhighlight lang="lua">local region_number = 10;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1289}}<syntaxhighlight lang="lua">player:SetStartingPlot(start_plot)</syntaxhighlight>
{{CodeLine5|1290}}<syntaxhighlight lang="lua">--print("Austria being placed in plot " .. x .. ", " .. y .. ".");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1292}}<syntaxhighlight lang="lua">-- Sweden</syntaxhighlight>
{{CodeLine5|1293}}<syntaxhighlight lang="lua">local region_number = 11;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1298}}<syntaxhighlight lang="lua">player:SetStartingPlot(start_plot)</syntaxhighlight>
{{CodeLine5|1299}}<syntaxhighlight lang="lua">--print("Sweden being placed in plot " .. x .. ", " .. y .. ".");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1301}}<syntaxhighlight lang="lua">-- Russia</syntaxhighlight>
{{CodeLine5|1302}}<syntaxhighlight lang="lua">local region_number = 12;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1307}}<syntaxhighlight lang="lua">player:SetStartingPlot(start_plot)</syntaxhighlight>
{{CodeLine5|1308}}<syntaxhighlight lang="lua">--print("Russia being placed in plot " .. x .. ", " .. y .. ".");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1310}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1237}}<syntaxhighlight lang="lua">pPlayer:SetStartingPlot(start_plot);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetStartingPlot]]
[[Category:Civ5 Players API|SetStartingPlot]]