{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:GetNumResource<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0323}}<syntaxhighlight lang="lua">strResourceText = strResourceText .. pResource.IconString .. " [COLOR_POSITIVE_TEXT]" .. Locale.ConvertTextKey(pResource.Description) .. " (" .. pTargetPlot:GetNumResource() .. ") [ENDCOLOR]";</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0327}}<syntaxhighlight lang="lua">tResourceList[iResourceType] = tResourceList[iResourceType] + pTargetPlot:GetNumResource();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0174}}<syntaxhighlight lang="lua">if (plot:GetNumResource() > 1) then</syntaxhighlight>
{{CodeLine5|0175}}<syntaxhighlight lang="lua">improvementStr = improvementStr .. plot:GetNumResource() .. " ";</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceTooltipGenerator.lua}}
:<code>UI/InGame/ResourceTooltipGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">strQuantity = plot:GetNumResource() .. " ";</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumResource]]
[[Category:Civ5 Resources API|GetNumResource]]