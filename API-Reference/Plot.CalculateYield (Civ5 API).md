{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:CalculateYield<b>(</b>{{Type5|YieldType}} index, '''bool''' display<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|index:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|display:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0268}}<syntaxhighlight lang="lua">iYieldChange = iYieldChange - pPlot:CalculateYield(iYield);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0384}}<syntaxhighlight lang="lua">local iNumFood = plot:CalculateYield(0, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0390}}<syntaxhighlight lang="lua">local iNumProduction = plot:CalculateYield(1, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0396}}<syntaxhighlight lang="lua">local iNumGold = plot:CalculateYield(2, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0402}}<syntaxhighlight lang="lua">local iNumScience = plot:CalculateYield(3, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0422}}<syntaxhighlight lang="lua">local iNumCulture = plot:CalculateYield(4, true);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0428}}<syntaxhighlight lang="lua">local iNumFaith = plot:CalculateYield(5, true);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|YieldIconManager.lua}}
:<code>UI/InGame/YieldIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">local iFood       = plot:CalculateYield( 0, true );-- + math.random( 0, 13 );</syntaxhighlight>
{{CodeLine5|0219}}<syntaxhighlight lang="lua">local iProduction = plot:CalculateYield( 1, true );-- + math.random( 0, 13 );</syntaxhighlight>
{{CodeLine5|0220}}<syntaxhighlight lang="lua">local iGold       = plot:CalculateYield( 2, true );-- + math.random( 0, 13 );</syntaxhighlight>
{{CodeLine5|0221}}<syntaxhighlight lang="lua">local iScience    = plot:CalculateYield( 3, true );-- + math.random( 0, 13 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|YieldIconManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/YieldIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0235}}<syntaxhighlight lang="lua">local iFood       = plot:CalculateYield( 0, true );</syntaxhighlight>
{{CodeLine5|0236}}<syntaxhighlight lang="lua">local iProduction = plot:CalculateYield( 1, true );</syntaxhighlight>
{{CodeLine5|0237}}<syntaxhighlight lang="lua">local iGold       = plot:CalculateYield( 2, true );</syntaxhighlight>
{{CodeLine5|0238}}<syntaxhighlight lang="lua">local iScience    = plot:CalculateYield( 3, true );</syntaxhighlight>
{{CodeLine5|0239}}<syntaxhighlight lang="lua">local iCulture    = plot:CalculateYield( 4, true );</syntaxhighlight>
{{CodeLine5|0240}}<syntaxhighlight lang="lua">local iFaith      = plot:CalculateYield( 5, true );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CalculateYield]]
[[Category:Civ5 Yields API|CalculateYield]]