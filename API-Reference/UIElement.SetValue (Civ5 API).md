{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Slider}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetValue<b>(</b>'''string''' sliderValue, {{Type5|PlayerID}} value = nil<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|sliderValue:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|value:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0948}}<syntaxhighlight lang="lua">Controls.MinorCivsSlider:SetValue( PreGame.GetNumMinorCivs() / maxMinorCivs );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0955}}<syntaxhighlight lang="lua">Controls.MinorCivsSlider:SetValue(0 / maxMinorCivs);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0958}}<syntaxhighlight lang="lua">Controls.MinorCivsSlider:SetValue(PreGame.GetNumMinorCivs() / maxMinorCivs);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0324}}<syntaxhighlight lang="lua">Controls.MinorCivsSlider:SetValue( 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0327}}<syntaxhighlight lang="lua">Controls.MinorCivsSlider:SetValue( PreGame.GetNumMinorCivs() / #GameInfo.MinorCivilizations );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0456}}<syntaxhighlight lang="lua">Controls.MusicVolumeSlider:SetValue(   GetVolumeKnobValue(iMusicVolumeKnobID) );</syntaxhighlight>
{{CodeLine5|0457}}<syntaxhighlight lang="lua">Controls.EffectsVolumeSlider:SetValue(   GetVolumeKnobValue(iSFXVolumeKnobID) );</syntaxhighlight>
{{CodeLine5|0458}}<syntaxhighlight lang="lua">Controls.SpeechVolumeSlider:SetValue(   GetVolumeKnobValue(iSpeechVolumeKnobID) );</syntaxhighlight>
{{CodeLine5|0459}}<syntaxhighlight lang="lua">Controls.AmbienceVolumeSlider:SetValue( GetVolumeKnobValue(iAmbienceVolumeKnobID) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0479}}<syntaxhighlight lang="lua">Controls.Tooltip1TimerSlider:SetValue(OptionsManager.GetTooltip1Seconds()/1000);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0711}}<syntaxhighlight lang="lua">Controls.Tooltip1TimerSlider:SetValue(OptionsManager.GetTooltip1Seconds_Cached()/1000);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0996}}<syntaxhighlight lang="lua">turnSlider:SetValue(sliderValue);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0777}}<syntaxhighlight lang="lua">savedData.SetValue("TurnsBetweenBonuses", 10);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0245}}<syntaxhighlight lang="lua">savedData.SetValue("WesternRomeCitiesCaptured", 0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0248}}<syntaxhighlight lang="lua">savedData.SetValue("EasternRomeCitiesCaptured", 0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0362}}<syntaxhighlight lang="lua">savedData.SetValue("HunCapturedFirstCity", 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0387}}<syntaxhighlight lang="lua">savedData.SetValue("WesternRomeCitiesCaptured", savedData.GetValue("WesternRomeCitiesCaptured") + 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0390}}<syntaxhighlight lang="lua">savedData.SetValue("EasternRomeCitiesCaptured", savedData.GetValue("EasternRomeCitiesCaptured") + 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2351}}<syntaxhighlight lang="lua">savedData.SetValue("InitializationComplete", 1);</syntaxhighlight>
{{CodeLine5|2352}}<syntaxhighlight lang="lua">savedData.SetValue("HunCapturedFirstCity", 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0032}}<syntaxhighlight lang="lua">g_SaveData.SetValue(name, value);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetValue]]