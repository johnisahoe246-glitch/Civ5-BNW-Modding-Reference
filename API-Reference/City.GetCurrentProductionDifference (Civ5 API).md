{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetCurrentProductionDifference<b>(</b>'''bool''' ignoreFood, '''bool''' overflow<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|ignoreFood:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|overflow:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|GameplayUtils.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/GameplayUtils.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0248}}<syntaxhighlight lang="lua">local iProd = pCity:GetCurrentProductionDifference(false, false);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WhosWinningPopup.lua}}
:<code>UI/InGame/Popups/WhosWinningPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0212}}<syntaxhighlight lang="lua">iTotalProduction = iTotalProduction + pLoopCity:GetCurrentProductionDifference(bIgnoreFood, bOverflow);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCurrentProductionDifference]]
[[Category:Civ5 City Production API|GetCurrentProductionDifference]]