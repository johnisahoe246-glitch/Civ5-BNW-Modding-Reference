{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Slider}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' UIElement:GetValue<b>(</b>'''string''' name = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|name:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|LoadTutorial.lua}}
:<code>UI/FrontEnd/LoadTutorial.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0232}}<syntaxhighlight lang="lua">local completed = modUserData.GetValue("Tutorial".. i .. "Completed");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0159}}<syntaxhighlight lang="lua">if (savedData.GetValue("FranceCatholic") == 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0163}}<syntaxhighlight lang="lua">if (savedData.GetValue("CeltsCatholic") == 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0167}}<syntaxhighlight lang="lua">if (savedData.GetValue("EnglandCatholic") == 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0171}}<syntaxhighlight lang="lua">if (savedData.GetValue("SpainCatholic") == 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0175}}<syntaxhighlight lang="lua">if (savedData.GetValue("NetherlandsCatholic") == 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0179}}<syntaxhighlight lang="lua">if (savedData.GetValue("AustriaCatholic") == 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0183}}<syntaxhighlight lang="lua">if (savedData.GetValue("SwedenCatholic") == 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0231}}<syntaxhighlight lang="lua">local iValue = savedData.GetValue("TurnsBetweenBonuses");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0244}}<syntaxhighlight lang="lua">iCitiesCaptured = savedData.GetValue("WesternRomeCitiesCaptured");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0247}}<syntaxhighlight lang="lua">iCitiesCaptured = savedData.GetValue("EasternRomeCitiesCaptured")</syntaxhighlight>
{{CodeLine5|0248}}<syntaxhighlight lang="lua">savedData.SetValue("EasternRomeCitiesCaptured", 0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0359}}<syntaxhighlight lang="lua">local iHunCitiesConquered = savedData.GetValue("HunCapturedFirstCity");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0387}}<syntaxhighlight lang="lua">savedData.SetValue("WesternRomeCitiesCaptured", savedData.GetValue("WesternRomeCitiesCaptured") + 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0390}}<syntaxhighlight lang="lua">savedData.SetValue("EasternRomeCitiesCaptured", savedData.GetValue("EasternRomeCitiesCaptured") + 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2338}}<syntaxhighlight lang="lua">local iValue = savedData.GetValue("InitializationComplete");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0021}}<syntaxhighlight lang="lua">g_Properties[name] = g_SaveData.GetValue(name);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UITestMenu.lua}}
:<code>UI/FrontEnd/UITestMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0088}}<syntaxhighlight lang="lua">Controls.BigSliderValue:SetText( "Big Slider: " .. Controls.BigSlider:GetValue() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">Controls.SmallSliderValue:SetText( "Small Slider: " .. Controls.SmallSlider:GetValue() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0675}}<syntaxhighlight lang="lua">local iVaticanExtraVoteTeam = g_savedData.GetValue("VaticanExtraVoteTeam");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetValue]]