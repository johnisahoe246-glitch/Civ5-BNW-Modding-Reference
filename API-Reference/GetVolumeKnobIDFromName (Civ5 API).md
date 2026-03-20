{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>{{Type5|ActionType}} GetVolumeKnobIDFromName<b>(</b>'''string''' arg0<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0034}}<syntaxhighlight lang="lua">local iMusicVolumeKnobID      = GetVolumeKnobIDFromName("USER_VOLUME_MUSIC");</syntaxhighlight>
{{CodeLine5|0035}}<syntaxhighlight lang="lua">local iSFXVolumeKnobID      = GetVolumeKnobIDFromName("USER_VOLUME_SFX");</syntaxhighlight>
{{CodeLine5|0036}}<syntaxhighlight lang="lua">local iSpeechVolumeKnobID      = GetVolumeKnobIDFromName("USER_VOLUME_SPEECH");</syntaxhighlight>
{{CodeLine5|0037}}<syntaxhighlight lang="lua">local iAmbienceVolumeKnobID   = GetVolumeKnobIDFromName("USER_VOLUME_AMBIENCE");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetVolumeKnobIDFromName]]