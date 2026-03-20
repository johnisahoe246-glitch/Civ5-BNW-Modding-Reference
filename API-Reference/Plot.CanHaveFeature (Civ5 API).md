{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:CanHaveFeature<b>(</b>{{Type5|FeatureType}} featureForest<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|featureForest:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0397}}<syntaxhighlight lang="lua">if plot:CanHaveFeature(featureForest) and forests:GetHeight(x, y) >= iForestLevel then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0402}}<syntaxhighlight lang="lua">if plot:CanHaveFeature(featureForest) and forests:GetHeight(x, y) >= iSEForestLevel then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">if plot:CanHaveFeature(self.featureFloodPlains) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0232}}<syntaxhighlight lang="lua">if(plot:CanHaveFeature(self.featureOasis)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0240}}<syntaxhighlight lang="lua">if(plot:CanHaveFeature(self.featureIce)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0259}}<syntaxhighlight lang="lua">if(plot:CanHaveFeature(self.featureMarsh)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0269}}<syntaxhighlight lang="lua">if(plot:CanHaveFeature(self.featureJungle)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0277}}<syntaxhighlight lang="lua">if plot:CanHaveFeature(self.featureForest) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0511}}<syntaxhighlight lang="lua">if plot:CanHaveFeature(featureFloodPlains) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0516}}<syntaxhighlight lang="lua">if (plot:CanHaveFeature(featureOasis)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0526}}<syntaxhighlight lang="lua">if (plot:CanHaveFeature(featureMarsh)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0540}}<syntaxhighlight lang="lua">elseif long > 0.72 and plot:CanHaveFeature(featureForest) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0545}}<syntaxhighlight lang="lua">if plot:CanHaveFeature(featureForest) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0588}}<syntaxhighlight lang="lua">if(plot:CanHaveFeature(feature.ID)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0740}}<syntaxhighlight lang="lua">if (plot:CanHaveFeature(self.featureIce)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanHaveFeature]]
[[Category:Civ5 Features & Natural wonders API|CanHaveFeature]]