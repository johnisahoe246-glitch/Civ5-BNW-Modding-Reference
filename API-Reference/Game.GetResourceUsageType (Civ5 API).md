{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|ResourceUsageType}} Game.GetResourceUsageType<b>(</b>{{Type5|ResourceType}} resourceLoop<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|resourceLoop:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|7507}}<syntaxhighlight lang="lua">if (Game.GetResourceUsageType(res_ID[use_this_res_index]) == ResourceUsageTypes.RESOURCEUSAGE_LUXURY) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0315}}<syntaxhighlight lang="lua">if (Game.GetResourceUsageType(iResourceType) ~= ResourceUsageTypes.RESOURCEUSAGE_BONUS) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0371}}<syntaxhighlight lang="lua">if (Game.GetResourceUsageType(iResourceLoop) ~= ResourceUsageTypes.RESOURCEUSAGE_BONUS) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericWorldAnchor.lua}}
:<code>UI/InGame/GenericWorldAnchor.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0156}}<syntaxhighlight lang="lua">local iUsage = Game.GetResourceUsageType(iResource);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0618}}<syntaxhighlight lang="lua">if (Game.GetResourceUsageType(iResourceID) ~= ResourceUsageTypes.RESOURCEUSAGE_BONUS) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceList.lua}}
:<code>UI/InGame/ResourceList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0096}}<syntaxhighlight lang="lua">if( Game.GetResourceUsageType( iResource ) == ResourceUsageTypes.RESOURCEUSAGE_STRATEGIC ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0102}}<syntaxhighlight lang="lua">if( Game.GetResourceUsageType( iResource ) == ResourceUsageTypes.RESOURCEUSAGE_LUXURY ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0107}}<syntaxhighlight lang="lua">if( Game.GetResourceUsageType( iResource ) == ResourceUsageTypes.RESOURCEUSAGE_BONUS ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0161}}<syntaxhighlight lang="lua">if (Game.GetResourceUsageType(iResourceLoop) == ResourceUsageTypes.RESOURCEUSAGE_STRATEGIC) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetResourceUsageType]]
[[Category:Civ5 Resources API|GetResourceUsageType]]