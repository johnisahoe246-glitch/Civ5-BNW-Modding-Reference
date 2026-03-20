{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Plot:SetFeatureType<b>(</b>'''int''' featureID, '''int''' arg1 = nil<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|featureID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 104 are listed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0398}}<syntaxhighlight lang="lua">plot:SetFeatureType(featureForest, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0407}}<syntaxhighlight lang="lua">plot:SetFeatureType(featureMarsh, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0437}}<syntaxhighlight lang="lua">plot:SetFeatureType(featureJungle, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5536}}<syntaxhighlight lang="lua">plot:SetFeatureType(wonder_list[1])</syntaxhighlight>
{{CodeLine5|5537}}<syntaxhighlight lang="lua">table.insert(self.placed_natural_wonder, 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5570}}<syntaxhighlight lang="lua">plot:SetFeatureType(wonder_list[2])</syntaxhighlight>
{{CodeLine5|5571}}<syntaxhighlight lang="lua">table.insert(self.placed_natural_wonder, 2);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5612}}<syntaxhighlight lang="lua">plot:SetFeatureType(wonder_list[3])</syntaxhighlight>
{{CodeLine5|5613}}<syntaxhighlight lang="lua">table.insert(self.placed_natural_wonder, 3);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5646}}<syntaxhighlight lang="lua">plot:SetFeatureType(wonder_list[4])</syntaxhighlight>
{{CodeLine5|5647}}<syntaxhighlight lang="lua">table.insert(self.placed_natural_wonder, 4);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5680}}<syntaxhighlight lang="lua">plot:SetFeatureType(wonder_list[5])</syntaxhighlight>
{{CodeLine5|5681}}<syntaxhighlight lang="lua">table.insert(self.placed_natural_wonder, 5);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5759}}<syntaxhighlight lang="lua">plot:SetFeatureType(wonder_list[6])</syntaxhighlight>
{{CodeLine5|5760}}<syntaxhighlight lang="lua">SEPlot:SetFeatureType(wonder_list[6])</syntaxhighlight>
{{CodeLine5|5761}}<syntaxhighlight lang="lua">table.insert(self.placed_natural_wonder, 6);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5801}}<syntaxhighlight lang="lua">plot:SetFeatureType(wonder_list[7])</syntaxhighlight>
{{CodeLine5|5802}}<syntaxhighlight lang="lua">table.insert(self.placed_natural_wonder, 7);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5832}}<syntaxhighlight lang="lua">plot:SetFeatureType(wonder_list[8])</syntaxhighlight>
{{CodeLine5|5833}}<syntaxhighlight lang="lua">table.insert(self.placed_natural_wonder, 8);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5839}}<syntaxhighlight lang="lua">plot:SetFeatureType(wonder_list[9])</syntaxhighlight>
{{CodeLine5|5840}}<syntaxhighlight lang="lua">table.insert(self.placed_natural_wonder, 9);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5845}}<syntaxhighlight lang="lua">plot:SetFeatureType(wonder_list[10])</syntaxhighlight>
{{CodeLine5|5846}}<syntaxhighlight lang="lua">table.insert(self.placed_natural_wonder, 10);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2858}}<syntaxhighlight lang="lua">forcePlot:SetFeatureType(FeatureTypes.NO_FEATURE, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3530}}<syntaxhighlight lang="lua">plot:SetFeatureType(FeatureTypes.FEATURE_OASIS, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3578}}<syntaxhighlight lang="lua">plot:SetFeatureType(FeatureTypes.NO_FEATURE, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5972}}<syntaxhighlight lang="lua">plot:SetFeatureType(feature_type_to_place)</syntaxhighlight>
{{CodeLine5|5973}}<syntaxhighlight lang="lua">table.insert(self.placed_natural_wonder, wonder_number);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9536}}<syntaxhighlight lang="lua">plot:SetFeatureType(FeatureTypes.FEATURE_MARSH, -1)</syntaxhighlight>
{{CodeLine5|9537}}<syntaxhighlight lang="lua">plot:SetTerrainType(TerrainTypes.TERRAIN_GRASS, false, true)</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Boreal.lua (G&K)}}
:<code>DLC/Expansion/Maps/Boreal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0567}}<syntaxhighlight lang="lua">plot:SetFeatureType(self.featureIce, -1)</syntaxhighlight>
{{CodeLine5|0568}}<syntaxhighlight lang="lua">elseif iY >= iH - 5 and plot:IsWater() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0583}}<syntaxhighlight lang="lua">plot:SetFeatureType(self.featureIce, -1)</syntaxhighlight>
{{CodeLine5|0584}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1171}}<syntaxhighlight lang="lua">plot:SetFeatureType(wonder_list[11])</syntaxhighlight>
{{CodeLine5|1172}}<syntaxhighlight lang="lua">table.insert(self.placed_natural_wonder, 11);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FeatureGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/FeatureGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0206}}<syntaxhighlight lang="lua">plot:SetFeatureType(self.featureFloodPlains, -1)</syntaxhighlight>
{{CodeLine5|0207}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0234}}<syntaxhighlight lang="lua">plot:SetFeatureType(self.featureOasis, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0242}}<syntaxhighlight lang="lua">plot:SetFeatureType(self.featureIce, -1)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0244}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0248}}<syntaxhighlight lang="lua">plot:SetFeatureType(self.featureIce, -1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0260}}<syntaxhighlight lang="lua">plot:SetFeatureType(self.featureMarsh, -1)</syntaxhighlight>
{{CodeLine5|0261}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0278}}<syntaxhighlight lang="lua">plot:SetFeatureType(self.featureForest, -1)</syntaxhighlight>
{{CodeLine5|0279}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0536}}<syntaxhighlight lang="lua">plot:SetFeatureType(feature_atoll, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0512}}<syntaxhighlight lang="lua">plot:SetFeatureType(featureFloodPlains, -1)</syntaxhighlight>
{{CodeLine5|0513}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0518}}<syntaxhighlight lang="lua">plot:SetFeatureType(featureOasis, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ice_Age.lua}}
:<code>Maps/Ice_Age.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0462}}<syntaxhighlight lang="lua">plot:SetFeatureType(self.featureIce, -1)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0464}}<syntaxhighlight lang="lua">elseif lat > 0.47 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0467}}<syntaxhighlight lang="lua">plot:SetFeatureType(self.featureIce, -1)</syntaxhighlight>
{{CodeLine5|0468}}<syntaxhighlight lang="lua">elseif rand < 4 * (lat - 0.46) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0591}}<syntaxhighlight lang="lua">plot:SetFeatureType(feature.ID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWondersCustomMethods.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/NaturalWondersCustomMethods.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0162}}<syntaxhighlight lang="lua">SEPlot:SetFeatureType(FeatureTypes.NO_FEATURE, -1)</syntaxhighlight>
{{CodeLine5|0163}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0197}}<syntaxhighlight lang="lua">SEPlot:SetFeatureType(feature_type_to_place);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Rainforest.lua (G&K)}}
:<code>DLC/Expansion/Maps/Rainforest.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0737}}<syntaxhighlight lang="lua">plot:SetFeatureType(self.featureJungle, -1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0276}}<syntaxhighlight lang="lua">plot:SetFeatureType(iFeatureID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetFeatureType]]
[[Category:Civ5 Features & Natural wonders API|SetFeatureType]]