{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' OptionsManager.GetTooltip1Seconds_Cached<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0665}}<syntaxhighlight lang="lua">Controls.Tooltip1TimerLength:SetText(Locale.ConvertTextKey("TXT_KEY_OPSCREEN_TOOLTIP_1_TIMER_LENGTH", math.floor(OptionsManager.GetTooltip1Seconds_Cached() / 100) ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0711}}<syntaxhighlight lang="lua">Controls.Tooltip1TimerSlider:SetValue(OptionsManager.GetTooltip1Seconds_Cached()/1000);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTooltip1Seconds_Cached]]