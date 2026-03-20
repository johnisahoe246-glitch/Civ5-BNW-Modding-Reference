{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:GetYield<b>(</b>{{Type5|YieldType}} index<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|index:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0148}}<syntaxhighlight lang="lua">iTotalFood = iTotalFood + pTargetPlot:GetYield(YieldTypes.YIELD_FOOD);</syntaxhighlight>
{{CodeLine5|0149}}<syntaxhighlight lang="lua">iTotalProduction = iTotalProduction + pTargetPlot:GetYield(YieldTypes.YIELD_PRODUCTION);</syntaxhighlight>
{{CodeLine5|0150}}<syntaxhighlight lang="lua">iTotalGold = iTotalGold + pTargetPlot:GetYield(YieldTypes.YIELD_GOLD);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetYield]]
[[Category:Civ5 Yields API|GetYield]]