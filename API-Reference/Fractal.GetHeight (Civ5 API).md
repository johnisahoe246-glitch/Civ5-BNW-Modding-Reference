{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Fractal}}.<br/>
This is an instance method, invoke it with a colon.<br/>
Used to get the value of the 2D fractal array or the value of a certain percentage of the array.
}}


=Usage=
<code>'''int''' Fractal:GetHeight<b>(</b>'''int''' percentage<b>)</b></code>

'''Returned Value'''
:Returns the threshold value of a percentage of the fractal array. For example, if you pass in 70, this function will return a number close to 178, give or take some depending on the breakdown of the values in the array. Seems to have trouble with smaller arrays (<10x10).
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|percentage:
|valign="top"| ''A number between 0 and 100.''
|}


<code>'''int''' Fractal:GetHeight<b>(</b>'''int''' x, '''int''' y<b>)</b></code>


'''Returned Value'''
:Returns the value of the fractal array at coordinates X, Y. The value is between 0 and 255.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''X coordinate of the value to retrieve.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''Y coordinate of the value to retrieve.''
|}

=Source code samples=
''Too many occurences. Only 50 out of 603 are listed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">local iHillsTop2 = hillsFrac:GetHeight(80);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0080}}<syntaxhighlight lang="lua">local iPeakAndes = peaksFrac:GetHeight(63);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0271}}<syntaxhighlight lang="lua">local iAndesGrass = grass_check:GetHeight(65)</syntaxhighlight>
{{CodeLine5|0272}}<syntaxhighlight lang="lua">local iAndesDesert = desert_check:GetHeight(75)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0312}}<syntaxhighlight lang="lua">local desertVal = desert_check:GetHeight(x, y);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0374}}<syntaxhighlight lang="lua">local iOpenLevel = open_lands:GetHeight(100 - iOpenPercent)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0376}}<syntaxhighlight lang="lua">local featureForest = FeatureTypes.FEATURE_FOREST;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0397}}<syntaxhighlight lang="lua">if plot:CanHaveFeature(featureForest) and forests:GetHeight(x, y) >= iForestLevel then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0418}}<syntaxhighlight lang="lua">if forests:GetHeight(x, y) >= iForestLevel then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0423}}<syntaxhighlight lang="lua">if marshes:GetHeight(x, y) >= iRiverMarshLevel then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">local iLakesThreshold = lakesFrac:GetHeight(94);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0138}}<syntaxhighlight lang="lua">local iHillsNearMountains = mountainsFrac:GetHeight(hillsNearMountains);</syntaxhighlight>
{{CodeLine5|0139}}<syntaxhighlight lang="lua">local iMountainThreshold = mountainsFrac:GetHeight(mountains);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0148}}<syntaxhighlight lang="lua">local lakeVal = lakesFrac:GetHeight(x,y);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">local hillVal = hillsFrac:GetHeight(x, y);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0184}}<syntaxhighlight lang="lua">local iSnowThreshold = snowFrac:GetHeight(65);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ContinentsWorld.lua}}
:<code>Gameplay/Lua/ContinentsWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0113}}<syntaxhighlight lang="lua">local iHillsTop2 = self.hillsFrac:GetHeight(75);</syntaxhighlight>
{{CodeLine5|0114}}<syntaxhighlight lang="lua">local iHillsClumps = self.mountainsFrac:GetHeight(4);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0447}}<syntaxhighlight lang="lua">local iGrassTop = grass_frac:GetHeight(iGrassPercent);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0520}}<syntaxhighlight lang="lua">local val = snow_frac:GetHeight(x, y);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0257}}<syntaxhighlight lang="lua">local marsh_height = self.marsh:GetHeight(iX, iY)</syntaxhighlight>
{{CodeLine5|0258}}<syntaxhighlight lang="lua">if(marsh_height >= self.iMarshLevel) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0276}}<syntaxhighlight lang="lua">if (self.forests:GetHeight(iX, iY) >= self.iForestLevel) or (self.forestclumps:GetHeight(iX, iY) >= self.iClumpLevel) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FractalWorld.lua}}
:<code>Gameplay/Lua/FractalWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0680}}<syntaxhighlight lang="lua">local iHillsBottom1 = self.hillsFrac:GetHeight(hillsBottom1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0693}}<syntaxhighlight lang="lua">local iMountain95 = self.mountainsFrac:GetHeight(95);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0717}}<syntaxhighlight lang="lua">local hillVal = self.hillsFrac:GetHeight(x, y);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">local iPlainsThreshold = hillsFrac:GetHeight(8);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">lat = lat + (128 - regionsFrac:GetHeight(x, y))/(255.0 * 5.0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0374}}<syntaxhighlight lang="lua">local iTexDesertBottom = plains:GetHeight(iTexDesertBottomPercent)</syntaxhighlight>
{{CodeLine5|0375}}<syntaxhighlight lang="lua">local iGrassTop = plains:GetHeight(iGrassTopPercent)</syntaxhighlight>
{{CodeLine5|0376}}<syntaxhighlight lang="lua">local iGrassBottom = plains:GetHeight(iGrassBottomPercent)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0379}}<syntaxhighlight lang="lua">local iEastDTop = east:GetHeight(iEastDTopPercent)</syntaxhighlight>
{{CodeLine5|0380}}<syntaxhighlight lang="lua">local iEastDBottom = east:GetHeight(iEastDBottomPercent)</syntaxhighlight>
{{CodeLine5|0381}}<syntaxhighlight lang="lua">local iEastPTop = east:GetHeight(iEastPTopPercent)</syntaxhighlight>
{{CodeLine5|0382}}<syntaxhighlight lang="lua">local iEastPBottom = east:GetHeight(iEastPBottomPercent)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0425}}<syntaxhighlight lang="lua">local val = east:GetHeight(x, y);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0497}}<syntaxhighlight lang="lua">local iRockyForestLevel = forests:GetHeight(iRockyForestPercent)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0499}}<syntaxhighlight lang="lua">local featureFloodPlains = FeatureTypes.FEATURE_FLOOD_PLAINS;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0541}}<syntaxhighlight lang="lua">if forests:GetHeight(x, y) <= iEastForestLevel then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1493}}<syntaxhighlight lang="lua">local iHerdsTop1 = herds:GetHeight(27)</syntaxhighlight>
{{CodeLine5|1494}}<syntaxhighlight lang="lua">local iHerdsBottom2 = herds:GetHeight(73)</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Hemispheres.lua (G&K)}}
:<code>DLC/Expansion/Maps/Hemispheres.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0822}}<syntaxhighlight lang="lua">local iHillsBottom1 = regionHillsFrac:GetHeight(20);</syntaxhighlight>
{{CodeLine5|0823}}<syntaxhighlight lang="lua">local iHillsTop1 = regionHillsFrac:GetHeight(35);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Highlands.lua}}
:<code>Maps/Highlands.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0180}}<syntaxhighlight lang="lua">local iHillsThreshold = terrainFrac:GetHeight(hills);</syntaxhighlight>
{{CodeLine5|0181}}<syntaxhighlight lang="lua">local iPeaksThreshold = terrainFrac:GetHeight(peaks);</syntaxhighlight>
{{CodeLine5|0182}}<syntaxhighlight lang="lua">local iPassThreshold = mountain_passFrac:GetHeight(85);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">local passVal = mountain_passFrac:GetHeight(x,y);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MultilayeredFractal.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MultilayeredFractal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0369}}<syntaxhighlight lang="lua">local iWaterThreshold = regionContinentsFrac:GetHeight(iWaterPercent);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0372}}<syntaxhighlight lang="lua">local iHillsBottom2 = regionHillsFrac:GetHeight(75 - adjustment);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0380}}<syntaxhighlight lang="lua">local val = regionContinentsFrac:GetHeight(x,y);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ring.lua}}
:<code>Maps/Ring.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0511}}<syntaxhighlight lang="lua">self.iForestLevel   = self.forests:GetHeight(80) -- 20% forest coverage</syntaxhighlight>
{{CodeLine5|0512}}<syntaxhighlight lang="lua">self.iClumpLevel   = self.forestclumps:GetHeight(94) -- 6% forest clumps</syntaxhighlight>
{{CodeLine5|0513}}<syntaxhighlight lang="lua">self.iMarshLevel   = self.marsh:GetHeight(100 - self.fMarshPercent)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0515}}<syntaxhighlight lang="lua">if dominant_terrain == 3 then -- Forest</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0517}}<syntaxhighlight lang="lua">self.iForestLevel   = self.forests:GetHeight(55) -- 45% forest coverage of what isn't covered by clumps.</syntaxhighlight>
{{CodeLine5|0518}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0307}}<syntaxhighlight lang="lua">elseif desertVal >= self.deserts:GetHeight(94) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TerrainGenerator.lua}}
:<code>Gameplay/Lua/TerrainGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0113}}<syntaxhighlight lang="lua">self.iDesertBottom = self.deserts:GetHeight(self.iDesertBottomPercent);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0119}}<syntaxhighlight lang="lua">self.iPlainsTop = self.plains:GetHeight(self.iPlainsTopPercent);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0183}}<syntaxhighlight lang="lua">local plainsVal = self.plains:GetHeight(iX, iY);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHeight]]