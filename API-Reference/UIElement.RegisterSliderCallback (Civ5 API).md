{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Slider}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:RegisterSliderCallback<b>(</b>('''void''' func<b>(</b>'''int''' fValue, {{Type5|ActionType}} void1<b>)</b>) OnMinorCivsSlider<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|OnMinorCivsSlider:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0935}}<syntaxhighlight lang="lua">Controls.MinorCivsSlider:RegisterSliderCallback( OnMinorCivsSlider );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0446}}<syntaxhighlight lang="lua">Controls.MusicVolumeSlider:RegisterSliderCallback(      OnUIVolumeSliderValueChanged );</syntaxhighlight>
{{CodeLine5|0447}}<syntaxhighlight lang="lua">Controls.EffectsVolumeSlider:RegisterSliderCallback(   OnUIVolumeSliderValueChanged );</syntaxhighlight>
{{CodeLine5|0448}}<syntaxhighlight lang="lua">Controls.SpeechVolumeSlider:RegisterSliderCallback(      OnUIVolumeSliderValueChanged );</syntaxhighlight>
{{CodeLine5|0449}}<syntaxhighlight lang="lua">Controls.AmbienceVolumeSlider:RegisterSliderCallback(   OnUIVolumeSliderValueChanged );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0478}}<syntaxhighlight lang="lua">Controls.Tooltip1TimerSlider:RegisterSliderCallback(Tooltip1TimerSliderChanged)</syntaxhighlight>
{{CodeLine5|0479}}<syntaxhighlight lang="lua">Controls.Tooltip1TimerSlider:SetValue(OptionsManager.GetTooltip1Seconds()/1000);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1194}}<syntaxhighlight lang="lua">Controls.TurnSlider:RegisterSliderCallback(OnTurnSliderValueChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UITestMenu.lua}}
:<code>UI/FrontEnd/UITestMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0086}}<syntaxhighlight lang="lua">Controls.BigSlider:RegisterSliderCallback( SliderUpdate );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0090}}<syntaxhighlight lang="lua">Controls.SmallSlider:RegisterSliderCallback( SliderUpdate );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RegisterSliderCallback]]