{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetEra<b>(</b>{{Type5|EraType}} id<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|id:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0490}}<syntaxhighlight lang="lua">PreGame.SetEra( id );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0796}}<syntaxhighlight lang="lua">PreGame.SetEra(wb.StartEra);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1236}}<syntaxhighlight lang="lua">PreGame.SetEra(era.ID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadTutorial.lua}}
:<code>UI/FrontEnd/LoadTutorial.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0097}}<syntaxhighlight lang="lua">PreGame.SetEra(0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MedievalScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/MedievalScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0055}}<syntaxhighlight lang="lua">PreGame.SetEra(2);   -- Medieval</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SteampunkScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/SteampunkScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0055}}<syntaxhighlight lang="lua">PreGame.SetEra(GameInfo.Eras["ERA_MODERN"].ID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetEra]]