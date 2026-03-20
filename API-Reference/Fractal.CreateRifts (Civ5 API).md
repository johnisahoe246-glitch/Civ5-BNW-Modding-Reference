{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Fractal}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|Fractal}} Fractal.CreateRifts<b>(</b>'''int''' regionWidth, '''int''' regionHeight, '''int''' continent_grain, '''table''' fracFlags, {{Type5|Fractal}} riftsFrac, '''float''' regionFracXExp, '''float''' regionFracYExp<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|regionWidth:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|regionHeight:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|continent_grain:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|fracFlags:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|riftsFrac:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|regionFracXExp:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|regionFracYExp:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|FractalWorld.lua}}
:<code>Gameplay/Lua/FractalWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0060}}<syntaxhighlight lang="lua">self.continentsFrac = Fractal.CreateRifts(self.iNumPlotsX, self.iNumPlotsY, continent_grain, fracFlags, self.riftsFrac, self.fracXExp, self.fracYExp);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MultilayeredFractal.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MultilayeredFractal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0339}}<syntaxhighlight lang="lua">regionContinentsFrac = Fractal.CreateRifts(iRegionWidth, iRegionHeight, iRegionGrain, iRegionPlotFlags, riftsFrac, iRegionFracXExp, iRegionFracYExp);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CreateRifts]]
[[Category:Civ5 City Production API|CreateRifts]]