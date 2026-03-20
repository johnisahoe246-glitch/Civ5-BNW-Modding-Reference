{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Map.GetNumResources<b>(</b>{{Type5|ResourceType}} resource<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|resource:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0070}}<syntaxhighlight lang="lua">if (((Map.GetNumResourcesOnLand(resourceID) * 100) / (Map.GetNumResources(resourceID) + 1)) < resource.MinLandPercent) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0164}}<syntaxhighlight lang="lua">if (Map.GetNumResources(resourceID) >= resourceCount) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0178}}<syntaxhighlight lang="lua">if (Map.GetNumResources(resourceID) < resourceCount) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumResources]]
[[Category:Civ5 Resources API|GetNumResources]]