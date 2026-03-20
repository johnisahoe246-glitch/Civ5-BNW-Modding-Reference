{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:CalculateTotalYield<b>(</b>{{Type5|YieldType}} yield<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|yield:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">return Players[iPlayer]:CalculateTotalYield(YieldTypes.YIELD_FOOD);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0188}}<syntaxhighlight lang="lua">return Players[iPlayer]:CalculateTotalYield(YieldTypes.YIELD_PRODUCTION);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CalculateTotalYield]]
[[Category:Civ5 Yields API|CalculateTotalYield]]
[[Category:Civ5 Score API|CalculateTotalYield]]