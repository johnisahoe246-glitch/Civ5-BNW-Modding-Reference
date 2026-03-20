{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.<br/>
Puts a resource on this plot.
}}


=Usage=
<code>'''void''' Plot:SetResourceType<b>(</b>{{Type5|ResourceType}} resourceID, '''int''' numResource<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|resourceID:
|valign="top"| ''The integer ID of the resource to place.''
|-
|valign="top" style="padding-right:6px;"|numResource:
|valign="top"| ''For strategic resources, this is the amount of that resource to place.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1421}}<syntaxhighlight lang="lua">res_plot:SetResourceType(selected_ID, selected_quantity);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|3492}}<syntaxhighlight lang="lua">plot:SetResourceType(self.banana_ID, 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3497}}<syntaxhighlight lang="lua">plot:SetResourceType(self.deer_ID, 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3502}}<syntaxhighlight lang="lua">plot:SetResourceType(self.sheep_ID, 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3509}}<syntaxhighlight lang="lua">plot:SetResourceType(self.cow_ID, 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3514}}<syntaxhighlight lang="lua">plot:SetResourceType(self.wheat_ID, 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3541}}<syntaxhighlight lang="lua">plot:SetResourceType(self.fish_ID, 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3610}}<syntaxhighlight lang="lua">plot:SetResourceType(choice, 2);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3613}}<syntaxhighlight lang="lua">plot:SetResourceType(self.iron_ID, 2);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3789}}<syntaxhighlight lang="lua">plot:SetResourceType(self.stone_ID, 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7506}}<syntaxhighlight lang="lua">res_plot:SetResourceType(res_ID[use_this_res_index], res_quantity[use_this_res_index]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|7663}}<syntaxhighlight lang="lua">res_plot:SetResourceType(resource_ID, quantity);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8930}}<syntaxhighlight lang="lua">res_plot:SetResourceType(self.marble_ID, 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|9146}}<syntaxhighlight lang="lua">res_plot:SetResourceType(self.fish_ID, 1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0173}}<syntaxhighlight lang="lua">plot:SetResourceType(resourceID, resourceNum);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0188}}<syntaxhighlight lang="lua">otherPlot:SetResourceType(resourceID, resourceNum);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0190}}<syntaxhighlight lang="lua">plot:SetResourceType(g_ResourcePlopper.ResourceType, g_ResourcePlopper.ResourceAmount);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0196}}<syntaxhighlight lang="lua">plot:SetResourceType(-1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0280}}<syntaxhighlight lang="lua">plot:SetResourceType(iResourceID, 5);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetResourceType]]
[[Category:Civ5 Resources API|SetResourceType]]