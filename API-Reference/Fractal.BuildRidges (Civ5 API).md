{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Fractal}}.<br/>
This is an instance method, invoke it with a colon.<br/>
Modifies a fractal to have randomized ridges.
}}


=Usage=
<code>'''void''' Fractal:BuildRidges<b>(</b>'''int''' numPlates, '''table''' flags, '''int''' xExponent, '''int''' yExponent<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|numPlates:
|valign="top"| ''The number of tectonic plates to use in generating the ridges. Where plates come into contact with each other, ridges are formed there.''
|-
|valign="top" style="padding-right:6px;"|flags:
|valign="top"| ''A table that holds certain additional options used in creating the fractal. See Fractal.Create().''
|-
|valign="top" style="padding-right:6px;"|xExponent:
|valign="top"| ''Amount of blurring to apply along X axis. 0 is no blur. 7 is high blur. Negative values sharpen?''
|-
|valign="top" style="padding-right:6px;"|yExponent:
|valign="top"| ''Amount of blurring to apply along Y axis. 0 is no blur. 7 is high blur. Negative values sharpen?''
|}

'''Example'''<br/>
This example will create a fractal and use it to build ridges based on the size of the map. It then loops through each value in the 2D fractal array and creates mountains if the value is greater than the highest 3% of all the values.
<syntaxhighlight lang="lua" class="civ5-example">
local iW, iH = Map.GetGridSize()
local mountains = Fractal.Create(iW, iH, 3, {FRAC_WRAP_X = true}, -1, -1)
mountains:BuildRidges((iW * iH) / 200, {}, 1, 1)
local mountainThreshold = mountains:GetHeight(97);
for y = 0, iH - 1 do
	for x = 0, iW - 1 do
		local height = mountains:GetHeight(x, y)
		--print (x .. ", " .. y .. ": " .. height)
		if height >= mountainThreshold then
			local plot = Map.GetPlot(x, y)
			plot:SetPlotType(PlotTypes.PLOT_MOUNTAIN, false, false)
		end
	end
end
</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0129}}<syntaxhighlight lang="lua">hillsFrac:BuildRidges(numPlates, iFlags, 1, 2);</syntaxhighlight>
{{CodeLine5|0130}}<syntaxhighlight lang="lua">mountainsFrac:BuildRidges((numPlates * 0.75), iFlags, 6, 1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ContinentsWorld.lua}}
:<code>Gameplay/Lua/ContinentsWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0100}}<syntaxhighlight lang="lua">self.hillsFrac:BuildRidges(numPlates, {FRAC_WRAP_X = true}, 1, 2);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">self.mountainsFrac:BuildRidges((numPlates * 2) / 3, {}, 6, 1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FractalWorld.lua}}
:<code>Gameplay/Lua/FractalWorld.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0090}}<syntaxhighlight lang="lua">self.continentsFrac:BuildRidges(numPlates, ridge_flags, 1, 2);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0674}}<syntaxhighlight lang="lua">self.hillsFrac:BuildRidges(numPlates, hills_ridge_flags, 1, 2);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0676}}<syntaxhighlight lang="lua">self.mountainsFrac:BuildRidges((numPlates * 2) / 3, peaks_ridge_flags, 6, 1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Highlands.lua}}
:<code>Maps/Highlands.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0174}}<syntaxhighlight lang="lua">mountain_passFrac:BuildRidges(numPlates, iFlags, 1, 2);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0176}}<syntaxhighlight lang="lua">terrainFrac:BuildRidges(numPlates, iFlags, 6, 1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|BuildRidges]]
[[Category:Civ5 Improvements API|BuildRidges]]