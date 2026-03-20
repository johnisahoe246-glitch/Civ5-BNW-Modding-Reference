{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>'''int''' GetVolumeKnobValue<b>(</b>{{Type5|ActionType}} musicVolumeKnob<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|musicVolumeKnob:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0045}}<syntaxhighlight lang="lua">m_cachedMusicVolumeKnob = GetVolumeKnobValue(iMusicVolumeKnobID);</syntaxhighlight>
{{CodeLine5|0046}}<syntaxhighlight lang="lua">m_cachedSFXVolumeKnob = GetVolumeKnobValue(iSFXVolumeKnobID);</syntaxhighlight>
{{CodeLine5|0047}}<syntaxhighlight lang="lua">m_cachedSpeechVolumeKnob = GetVolumeKnobValue(iSpeechVolumeKnobID);</syntaxhighlight>
{{CodeLine5|0048}}<syntaxhighlight lang="lua">m_cachedAmbienceVolumeKnob = GetVolumeKnobValue(iAmbienceVolumeKnobID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0409}}<syntaxhighlight lang="lua">fRealVolume = GetVolumeKnobValue(iVolumeKnobID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0456}}<syntaxhighlight lang="lua">Controls.MusicVolumeSlider:SetValue(   GetVolumeKnobValue(iMusicVolumeKnobID) );</syntaxhighlight>
{{CodeLine5|0457}}<syntaxhighlight lang="lua">Controls.EffectsVolumeSlider:SetValue(   GetVolumeKnobValue(iSFXVolumeKnobID) );</syntaxhighlight>
{{CodeLine5|0458}}<syntaxhighlight lang="lua">Controls.SpeechVolumeSlider:SetValue(   GetVolumeKnobValue(iSpeechVolumeKnobID) );</syntaxhighlight>
{{CodeLine5|0459}}<syntaxhighlight lang="lua">Controls.AmbienceVolumeSlider:SetValue( GetVolumeKnobValue(iAmbienceVolumeKnobID) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0461}}<syntaxhighlight lang="lua">Controls.MusicVolumeSliderValue:SetText( Locale.ConvertTextKey("TXT_KEY_OPSCREEN_MUSIC_SLIDER", math.floor(GetVolumeKnobValue(iMusicVolumeKnobID)*100) ) );</syntaxhighlight>
{{CodeLine5|0462}}<syntaxhighlight lang="lua">Controls.EffectsVolumeSliderValue:SetText( Locale.ConvertTextKey("TXT_KEY_OPSCREEN_SF_SLIDER", math.floor(GetVolumeKnobValue(iSFXVolumeKnobID)*100) ) );</syntaxhighlight>
{{CodeLine5|0463}}<syntaxhighlight lang="lua">Controls.SpeechVolumeSliderValue:SetText( Locale.ConvertTextKey("TXT_KEY_OPSCREEN_SPEECH_SLIDER", math.floor(GetVolumeKnobValue(iSpeechVolumeKnobID)*100) ) );</syntaxhighlight>
{{CodeLine5|0464}}<syntaxhighlight lang="lua">Controls.AmbienceVolumeSliderValue:SetText( Locale.ConvertTextKey("TXT_KEY_OPSCREEN_AMBIANCE_SLIDER", math.floor(GetVolumeKnobValue(iAmbienceVolumeKnobID)*100) ) );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetVolumeKnobValue]]