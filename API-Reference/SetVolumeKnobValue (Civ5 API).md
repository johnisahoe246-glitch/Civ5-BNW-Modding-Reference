{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>'''void''' SetVolumeKnobValue<b>(</b>{{Type5|ActionType}} musicVolumeKnob, '''int''' cachedMusicVolumeKnob<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|musicVolumeKnob:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|cachedMusicVolumeKnob:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0056}}<syntaxhighlight lang="lua">SetVolumeKnobValue(iMusicVolumeKnobID, m_cachedMusicVolumeKnob);</syntaxhighlight>
{{CodeLine5|0057}}<syntaxhighlight lang="lua">SetVolumeKnobValue(iSFXVolumeKnobID, m_cachedSFXVolumeKnob);</syntaxhighlight>
{{CodeLine5|0058}}<syntaxhighlight lang="lua">SetVolumeKnobValue(iSpeechVolumeKnobID, m_cachedSpeechVolumeKnob);</syntaxhighlight>
{{CodeLine5|0059}}<syntaxhighlight lang="lua">SetVolumeKnobValue(iAmbienceVolumeKnobID, m_cachedAmbienceVolumeKnob);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0080}}<syntaxhighlight lang="lua">SetVolumeKnobValue(iMusicVolumeKnobID, 1);</syntaxhighlight>
{{CodeLine5|0081}}<syntaxhighlight lang="lua">SetVolumeKnobValue(iSFXVolumeKnobID, 1);</syntaxhighlight>
{{CodeLine5|0082}}<syntaxhighlight lang="lua">SetVolumeKnobValue(iSpeechVolumeKnobID, 1);</syntaxhighlight>
{{CodeLine5|0083}}<syntaxhighlight lang="lua">SetVolumeKnobValue(iAmbienceVolumeKnobID, 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0428}}<syntaxhighlight lang="lua">SetVolumeKnobValue(void1, fNewVolumeLevel);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetVolumeKnobValue]]