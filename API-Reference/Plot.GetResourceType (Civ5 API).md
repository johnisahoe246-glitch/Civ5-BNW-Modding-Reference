{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|ResourceType}} Plot:GetResourceType<b>(</b>{{Type5|TeamID}} team<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|team:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1322}}<syntaxhighlight lang="lua">if res_plot:GetResourceType(-1) == -1 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|3475}}<syntaxhighlight lang="lua">if plot:GetResourceType(-1) ~= -1 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4268}}<syntaxhighlight lang="lua">if plot:GetResourceType(-1) == -1 then -- No resource here, safe to proceed.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7137}}<syntaxhighlight lang="lua">elseif plot:GetResourceType(-1) ~= -1 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7500}}<syntaxhighlight lang="lua">if res_plot:GetResourceType(-1) == -1 then -- Placing this strategic resource in this plot.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7520}}<syntaxhighlight lang="lua">if res_plot:GetResourceType(-1) == -1 then -- Placing this luxury resource in this plot.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7537}}<syntaxhighlight lang="lua">if res_plot:GetResourceType(-1) == -1 then -- Placing this bonus resource in this plot.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7662}}<syntaxhighlight lang="lua">if res_plot:GetResourceType(-1) == -1 then -- Placing this resource in this plot.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9207}}<syntaxhighlight lang="lua">if plot:GetResourceType(-1) == -1 and featureType ~= FeatureTypes.FEATURE_OASIS then -- No resource or Oasis here, safe to proceed.</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9360}}<syntaxhighlight lang="lua">if plot:GetResourceType(-1) == -1 then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9529}}<syntaxhighlight lang="lua">if plot:GetResourceType(-1) == self.sugar_ID then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0311}}<syntaxhighlight lang="lua">local iResourceType = pTargetPlot:GetResourceType(Game.GetActiveTeam());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">local iResource = pTargetPlot:GetResourceType(iActiveTeam);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0242}}<syntaxhighlight lang="lua">local iResource = pPlot:GetResourceType(Game.GetActiveTeam());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1510}}<syntaxhighlight lang="lua">elseif plot:GetResourceType(-1) == -1 then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0613}}<syntaxhighlight lang="lua">if (plot:GetResourceType() ~= NO_RESOURCE) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0170}}<syntaxhighlight lang="lua">if (plot:GetResourceType(iActiveTeam) >= 0) then</syntaxhighlight>
{{CodeLine5|0171}}<syntaxhighlight lang="lua">local resourceType = plot:GetResourceType(iActiveTeam);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceTooltipGenerator.lua}}
:<code>UI/InGame/ResourceTooltipGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0006}}<syntaxhighlight lang="lua">local iResourceID = plot:GetResourceType(Game.GetActiveTeam());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1276}}<syntaxhighlight lang="lua">local iResourceID = pPlot:GetResourceType(iActiveTeam);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1280}}<syntaxhighlight lang="lua">local pResource = GameInfo.Resources[pPlot:GetResourceType(iActiveTeam)];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0063}}<syntaxhighlight lang="lua">if ((otherPlot:GetResourceType() ~= -1) and (otherPlot:GetResourceType() ~= resourceID)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0091}}<syntaxhighlight lang="lua">local otherResource = GameInfo.Resources[otherPlot:GetResourceType()];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0116}}<syntaxhighlight lang="lua">if (otherPlot:GetResourceType() == resourceID) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetResourceType]]
[[Category:Civ5 Resources API|GetResourceType]]