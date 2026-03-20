{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetScoreFromFutureTech<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0200}}<syntaxhighlight lang="lua">strMyScoreTooltip = strMyScoreTooltip .. Locale.ConvertTextKey("TXT_KEY_DIPLO_MY_SCORE_FUTURE_TECH", g_pPlayer:GetScoreFromFutureTech());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0183}}<syntaxhighlight lang="lua">Controls.FutureTech:SetText(pPlayer:GetScoreFromFutureTech());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetScoreFromFutureTech]]
[[Category:Civ5 Science API|GetScoreFromFutureTech]]
[[Category:Civ5 Score API|GetScoreFromFutureTech]]