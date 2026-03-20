{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:CalculateGrossGoldTimes100<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0193}}<syntaxhighlight lang="lua">Controls.GrossGoldValue:SetText( "[COLOR_POSITIVE_TEXT]" .. Locale.ToNumber( pPlayer:CalculateGrossGoldTimes100() / 100, "#.##" ) .. "[ENDCOLOR]" );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CalculateGrossGoldTimes100]]
[[Category:Civ5 Gold API|CalculateGrossGoldTimes100]]