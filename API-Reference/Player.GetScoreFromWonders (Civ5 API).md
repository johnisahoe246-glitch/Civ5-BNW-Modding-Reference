{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetScoreFromWonders<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0196}}<syntaxhighlight lang="lua">strMyScoreTooltip = strMyScoreTooltip .. Locale.ConvertTextKey("TXT_KEY_DIPLO_MY_SCORE_WONDERS", g_pPlayer:GetScoreFromWonders());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryProgress.lua}}
:<code>UI/InGame/Popups/VictoryProgress.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0181}}<syntaxhighlight lang="lua">Controls.Wonders:SetText(pPlayer:GetScoreFromWonders());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetScoreFromWonders]]
[[Category:Civ5 Buildings API|GetScoreFromWonders]]
[[Category:Civ5 Score API|GetScoreFromWonders]]