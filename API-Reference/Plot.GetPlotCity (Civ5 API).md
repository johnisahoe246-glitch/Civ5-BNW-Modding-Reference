{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:GetPlotCity<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Too many occurences. Only 50 out of 197 are listed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0953}}<syntaxhighlight lang="lua">local city = plot:GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1098}}<syntaxhighlight lang="lua">if (plot:GetPlotCity():IsPuppet()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1807}}<syntaxhighlight lang="lua">local pCity = pPlot:GetPlotCity();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0386}}<syntaxhighlight lang="lua">city = plot:GetPlotCity();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0336}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(19,55):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0342}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(29,73):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0346}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(56,69):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0358}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(61,50):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0366}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(40,1):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0377}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(43,17):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0420}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(36,16):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0434}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(42,26):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0443}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(41,10):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0446}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(39,18):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0449}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(49,21):GetPlotCity();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0452}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(35,27):GetPlotCity();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1534}}<syntaxhighlight lang="lua">local pCity = Map.GetPlot(iX, iY):GetPlotCity();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0503}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(10,16):GetPlotCity(); -- Russadir</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0505}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(15,18):GetPlotCity(); -- Iol Caesarea</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0515}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(37,27):GetPlotCity(); -- Neapoli</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0517}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(41,27):GetPlotCity(); -- Brundisium</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0521}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(6,29):GetPlotCity();  -- Emerita Augusta</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0525}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(33,31):GetPlotCity(); -- Rome</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0527}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(14,34):GetPlotCity(); -- Caesaraugusta</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0529}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(20,36):GetPlotCity(); -- Narbo</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0539}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(3,39):GetPlotCity();  -- Brigantium</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0541}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(30,40):GetPlotCity(); -- Milan</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0545}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(22,42):GetPlotCity(); -- Lundunum</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0547}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(32,45):GetPlotCity(); -- Casta Regina</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0555}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(26,49):GetPlotCity(); -- Trier</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0557}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(17,52):GetPlotCity(); -- Coriallum</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0567}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(48,7):GetPlotCity();  -- Cyrene</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0579}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(73,20):GetPlotCity(); -- Antioch</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0581}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(63,21):GetPlotCity(); -- Attalia</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0583}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(76,21):GetPlotCity(); -- Edessa</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0585}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(51,22):GetPlotCity(); -- Athens</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0587}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(47,23):GetPlotCity(); -- Nicopolis</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0591}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(67,24):GetPlotCity(); -- Iconium</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0593}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(75,26):GetPlotCity(); -- Melitene</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0599}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(58,29):GetPlotCity(); -- Constantinople</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0601}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(45,30):GetPlotCity(); -- Dyrrachium</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0603}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(71,30):GetPlotCity(); -- Amasia</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0607}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(64,32):GetPlotCity(); -- Amastris</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0611}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(49,34):GetPlotCity(); -- Naissus</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0623}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(87,17):GetPlotCity(); -- Ctesiphon</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0629}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(79,24):GetPlotCity(); -- Amida</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0633}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(81,33):GetPlotCity(); -- Anium</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0955}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(1,15):GetPlotCity(); -- Tricameron</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0959}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(4,19):GetPlotCity(); -- Caput Vada</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0963}}<syntaxhighlight lang="lua">pCity = Map.GetPlot(84, 58):GetPlotCity(); -- Attila's Court</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetPlotCity]]
[[Category:Civ5 Cities API|GetPlotCity]]