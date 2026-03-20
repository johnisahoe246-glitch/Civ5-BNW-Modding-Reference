{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' PreGame.GetLoadWBScenario<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">PreGame.SetLoadWBScenario(PreGame.GetLoadWBScenario());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">PreGame.SetLoadWBScenario(not PreGame.GetLoadWBScenario());</syntaxhighlight>
{{CodeLine5|0153}}<syntaxhighlight lang="lua">if(PreGame.GetLoadWBScenario()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0373}}<syntaxhighlight lang="lua">if (PreGame.GetLoadWBScenario() and not bScenarioSettingsLoaded) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0395}}<syntaxhighlight lang="lua">if (PreGame.GetLoadWBScenario() and IsWBMap(mapFileName)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0431}}<syntaxhighlight lang="lua">local loadScenarioChecked = PreGame.GetLoadWBScenario();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">g_bIsScenario = (PreGame.GetLoadWBScenario() and isWBMap);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetLoadWBScenario]]
[[Category:Civ5 Movement API|GetLoadWBScenario]]