{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ButtonBase''' and {{Type5|Slider}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|ActionType}} UIElement:GetVoid1<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6461}}<syntaxhighlight lang="lua">local id = control:GetVoid1();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0415}}<syntaxhighlight lang="lua">if Controls.MusicVolumeSlider:GetVoid1() == iVolumeKnobID then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0417}}<syntaxhighlight lang="lua">elseif Controls.EffectsVolumeSlider:GetVoid1() == iVolumeKnobID then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0419}}<syntaxhighlight lang="lua">elseif Controls.SpeechVolumeSlider:GetVoid1() == iVolumeKnobID then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0421}}<syntaxhighlight lang="lua">elseif Controls.AmbienceVolumeSlider:GetVoid1() == iVolumeKnobID then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0435}}<syntaxhighlight lang="lua">if Controls.MusicVolumeSlider:GetVoid1() == void1 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0437}}<syntaxhighlight lang="lua">elseif Controls.EffectsVolumeSlider:GetVoid1() == void1 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0439}}<syntaxhighlight lang="lua">elseif Controls.SpeechVolumeSlider:GetVoid1() == void1 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0441}}<syntaxhighlight lang="lua">elseif Controls.AmbienceVolumeSlider:GetVoid1() == void1 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1924}}<syntaxhighlight lang="lua">if( control:GetVoid1() == 1 ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2313}}<syntaxhighlight lang="lua">local bIsUs = control:GetVoid1() == 1;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0847}}<syntaxhighlight lang="lua">local iAction = control:GetVoid1();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetVoid1]]