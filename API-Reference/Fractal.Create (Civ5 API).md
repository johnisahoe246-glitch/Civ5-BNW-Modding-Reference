{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Fractal}}.<br/>
This is a static method, invoke it with a dot.<br/>
Used to create a 2D-array of random values using [Fractal] (insert wikipedia link here) math.
}}


=Usage=
<code>{{Type5|Fractal}} Fractal.Create<b>(</b>'''int''' width, '''int''' height, '''int''' grain, '''table''' fractalFlags, '''int''' xExponent, '''int''' yExponent<b>)</b></code>


'''Returned Value'''
:Returns an instance of Fractal.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|width:
|valign="top"| ''The width of the 2D array to create.''
|-
|valign="top" style="padding-right:6px;"|height:
|valign="top"| ''The height of the 2D array to create.''
|-
|valign="top" style="padding-right:6px;"|grain:
|valign="top"| ''Amount of grain to add to fractal. 0 is no grain (smooth), 7 is lots of grain (jagged).''
|-
|valign="top" style="padding-right:6px;"|fractalFlags:
|valign="top"| ''A table that holds certain additional options used in creating the fractal. See below.''
|-
|valign="top" style="padding-right:6px;"|xExponent:
|valign="top"| ''Width resolution of the fractal. Higher values will produce sharper fractals, while lower values will produce blurry ones.''
|-
|valign="top" style="padding-right:6px;"|yExponent:
|valign="top"| ''Height resolution of the fractal.''
|}

'''A note about fractal exponents from MultilayeredFractal.lua:'''
<blockquote>FracXExp is the width of the source fractal.
FracYExp is the height of the source fractal.
These exponents are raised to powers of two. So a value of FracXExp = 7 
means 2^7, which would be 128 units wide. FracXExp = 6 would be only 64 
units wide. FracYExp works the same way.</blockquote>

'''Fractal Flags'''
:{|
|-
|valign="top" style="padding-right:6px;"|'''boolean''' FRAC_WRAP_X:
|valign="top"| ''Whether or not the fractal should wrap around the X axis.''
|-
|valign="top" style="padding-right:6px;"|'''boolean''' FRAC_WRAP_Y:
|valign="top"| ''???''
|-
|valign="top" style="padding-right:6px;"|'''boolean''' FRAC_POLAR:
|valign="top"| ''???''
|}

=Source code samples=
''Too many occurences. Only 50 out of 130 are listed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">local peaksFrac = Fractal.Create(iW, iH, grain_amount + 1, {}, 6, 6);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0269}}<syntaxhighlight lang="lua">local grass_check = Fractal.Create(iW, iH, 5, {}, 6, 6);</syntaxhighlight>
{{CodeLine5|0270}}<syntaxhighlight lang="lua">local desert_check = Fractal.Create(iW, iH, 4, {}, 6, 6);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0366}}<syntaxhighlight lang="lua">local marshes = Fractal.Create(iW, iH, forest_grain, {}, 6, 6);</syntaxhighlight>
{{CodeLine5|0367}}<syntaxhighlight lang="lua">local forests = Fractal.Create(iW, iH, forest_grain, {}, 6, 6);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0126}}<syntaxhighlight lang="lua">local lakesFrac = Fractal.Create(iW, iH, 2, iFlags, -1, -1);</syntaxhighlight>
{{CodeLine5|0127}}<syntaxhighlight lang="lua">local hillsFrac = Fractal.Create(iW, iH, grain, iFlags, -1, -1);</syntaxhighlight>
{{CodeLine5|0128}}<syntaxhighlight lang="lua">local mountainsFrac = Fractal.Create(iW, iH, grain, iFlags, -1, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0181}}<syntaxhighlight lang="lua">local snowFrac = Fractal.Create(iW, iH, 3, iFlags, -1, -1);</syntaxhighlight>
{{CodeLine5|0182}}<syntaxhighlight lang="lua">local snowFrac2 = Fractal.Create(iW, 1 + math.floor(iH * 0.4), 2, iFlags, 7, 6);</syntaxhighlight>
{{CodeLine5|0183}}<syntaxhighlight lang="lua">local plainsFrac = Fractal.Create(iW, iH, 4, iFlags, -1, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ContinentsWorld.lua}}
:<code>Gameplay/Lua/ContinentsWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0102}}<syntaxhighlight lang="lua">self.mountainsFrac = Fractal.Create(self.iNumPlotsX, self.iNumPlotsY, 4, self.iFlags, self.fracXExp, self.fracYExp);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0440}}<syntaxhighlight lang="lua">local snow_frac = Fractal.Create(iW, iH, grain_amount + 1, iFlags, -1, -1);</syntaxhighlight>
{{CodeLine5|0441}}<syntaxhighlight lang="lua">local tundra_frac = Fractal.Create(iW, iH, grain_amount + 1, iFlags, -1, -1);</syntaxhighlight>
{{CodeLine5|0442}}<syntaxhighlight lang="lua">local grass_frac = Fractal.Create(iW, iH, grain_amount, iFlags, -1, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0128}}<syntaxhighlight lang="lua">self.jungles      = Fractal.Create(width, height, self.jungle_grain, self.fractalFlags, self.fracXExp, self.fracYExp);</syntaxhighlight>
{{CodeLine5|0129}}<syntaxhighlight lang="lua">self.forests      = Fractal.Create(width, height, self.forest_grain, self.fractalFlags, self.fracXExp, self.fracYExp);</syntaxhighlight>
{{CodeLine5|0130}}<syntaxhighlight lang="lua">self.forestclumps   = Fractal.Create(width, height, self.clump_grain, self.fractalFlags, self.fracXExp, self.fracYExp);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FractalWorld.lua}}
:<code>Gameplay/Lua/FractalWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0059}}<syntaxhighlight lang="lua">self.riftsFrac = Fractal.Create(self.iNumPlotsX, self.iNumPlotsY, rift_grain, {}, self.fracXExp, self.fracYExp);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0062}}<syntaxhighlight lang="lua">self.continentsFrac = Fractal.Create(self.iNumPlotsX, self.iNumPlotsY, continent_grain, fracFlags, self.fracXExp, self.fracYExp);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0662}}<syntaxhighlight lang="lua">self.hillsFrac = Fractal.Create(self.iNumPlotsX, self.iNumPlotsY, grain, self.iFlags, self.fracXExp, self.fracYExp);</syntaxhighlight>
{{CodeLine5|0663}}<syntaxhighlight lang="lua">self.mountainsFrac = Fractal.Create(self.iNumPlotsX, self.iNumPlotsY, grain, self.iFlags, self.fracXExp, self.fracYExp);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">local hillsFrac = Fractal.Create(iW, iH, grain_amount, iFlags, 6, 6);</syntaxhighlight>
{{CodeLine5|0070}}<syntaxhighlight lang="lua">local peaksFrac = Fractal.Create(iW, iH, grain_amount + 1, iFlags, 6, 6);</syntaxhighlight>
{{CodeLine5|0071}}<syntaxhighlight lang="lua">local regionsFrac = Fractal.Create(iW, iH, grain_amount, iFlags, 6, 6);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0361}}<syntaxhighlight lang="lua">local rocky = Fractal.Create(iW, iH, grain_amount, iFlags, -1, -1);</syntaxhighlight>
{{CodeLine5|0362}}<syntaxhighlight lang="lua">local plains = Fractal.Create(iW, iH, grain_amount + 1, iFlags, -1, -1);</syntaxhighlight>
{{CodeLine5|0363}}<syntaxhighlight lang="lua">local east = Fractal.Create(iW, iH, grain_amount, iFlags, -1, -1);</syntaxhighlight>
{{CodeLine5|0364}}<syntaxhighlight lang="lua">local variation = Fractal.Create(iW, iH, grain_amount, iFlags, -1, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0492}}<syntaxhighlight lang="lua">local forests = Fractal.Create(iW, iH, forest_grain, iFlags, fracXExp, fracYExp);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1490}}<syntaxhighlight lang="lua">local herds = Fractal.Create(iW, iH, 7, {}, -1, -1)</syntaxhighlight>
{{CodeLine5|1491}}<syntaxhighlight lang="lua">local iHerdsClumps = herds:GetHeight(3)</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Hemispheres.lua (G&K)}}
:<code>DLC/Expansion/Maps/Hemispheres.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0820}}<syntaxhighlight lang="lua">local regionHillsFrac = Fractal.Create(iW, iH, 5, {}, 7, 7);</syntaxhighlight>
{{CodeLine5|0821}}<syntaxhighlight lang="lua">local regionPeaksFrac = Fractal.Create(iW, iH, 6, {}, 7, 7);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Highlands.lua}}
:<code>Maps/Highlands.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0169}}<syntaxhighlight lang="lua">local terrainFrac = Fractal.Create(iW, iH, grain, iFlags, -1, -1);</syntaxhighlight>
{{CodeLine5|0170}}<syntaxhighlight lang="lua">local lakesFrac = Fractal.Create(iW, iH, lake_grain, iFlags, -1, -1);</syntaxhighlight>
{{CodeLine5|0171}}<syntaxhighlight lang="lua">local mountain_passFrac = Fractal.Create(iW, iH, grain, iFlags, -1, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InlandSea.lua}}
:<code>Maps/InlandSea.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">local seaFrac = Fractal.Create(iWidth, iHeight, grain, fracFlags, -1, -1)</syntaxhighlight>
{{CodeLine5|0074}}<syntaxhighlight lang="lua">local seaThreshold = seaFrac:GetHeight(47);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lakes.lua}}
:<code>Maps/Lakes.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0100}}<syntaxhighlight lang="lua">local lakesFrac = Fractal.Create(iW, iH, lake_grain, fracFlags, -1, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MultilayeredFractal.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MultilayeredFractal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0338}}<syntaxhighlight lang="lua">local riftsFrac = Fractal.Create(iRegionWidth, iRegionHeight, iRiftGrain, {}, iRegionFracXExp, iRegionFracYExp);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0341}}<syntaxhighlight lang="lua">regionContinentsFrac = Fractal.Create(iRegionWidth, iRegionHeight, iRegionGrain, iRegionPlotFlags, iRegionFracXExp, iRegionFracYExp);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0350}}<syntaxhighlight lang="lua">local regionHillsFrac = Fractal.Create(iRegionWidth, iRegionHeight, iRegionHillsGrain, iRegionTerrainFlags, iRegionFracXExp, iRegionFracYExp);</syntaxhighlight>
{{CodeLine5|0351}}<syntaxhighlight lang="lua">local regionPeaksFrac = Fractal.Create(iRegionWidth, iRegionHeight, iRegionHillsGrain + 1, iRegionTerrainFlags, iRegionFracXExp, iRegionFracYExp);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0708}}<syntaxhighlight lang="lua">self.hillsFrac = Fractal.Create(self.iW, self.iH, grain_amount, self.iTerrainFlags, fracXExp, fracYExp);</syntaxhighlight>
{{CodeLine5|0709}}<syntaxhighlight lang="lua">self.mountainsFrac = Fractal.Create(self.iW, self.iH, grain_amount, self.iTerrainFlags, fracXExp, fracYExp);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|North_vs_South.lua}}
:<code>Maps/North_vs_South.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0090}}<syntaxhighlight lang="lua">local lakesFrac = Fractal.Create(iW, iH, lake_grain, fracFlags, 6, 6);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Oval.lua}}
:<code>Maps/Oval.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0100}}<syntaxhighlight lang="lua">local baysFrac = Fractal.Create(iW, iH, 3, fracFlags, -1, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0146}}<syntaxhighlight lang="lua">local terrainFrac = Fractal.Create(iW, iH, grain, fracFlags, -1, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0151}}<syntaxhighlight lang="lua">local hillsFrac = Fractal.Create(iW, iH, grain, fracFlags, -1, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TerrainGenerator.lua}}
:<code>Gameplay/Lua/TerrainGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0108}}<syntaxhighlight lang="lua">self.deserts = Fractal.Create(   self.iWidth, self.iHeight,</syntaxhighlight>
{{CodeLine5|0109}}<syntaxhighlight lang="lua">self.grain_amount, self.fractalFlags,</syntaxhighlight>
{{CodeLine5|0110}}<syntaxhighlight lang="lua">self.fracXExp, self.fracYExp);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">self.plains = Fractal.Create(   self.iWidth, self.iHeight,</syntaxhighlight>
{{CodeLine5|0116}}<syntaxhighlight lang="lua">self.grain_amount, self.fractalFlags,</syntaxhighlight>
{{CodeLine5|0117}}<syntaxhighlight lang="lua">self.fracXExp, self.fracYExp);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Create]]
[[Category:Civ5 City Production API|Create]]