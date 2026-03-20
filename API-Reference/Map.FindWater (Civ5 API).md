{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Map}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' Map.FindWater<b>(</b>{{Type5|Plot}} plot, '''int''' range, '''bool''' isFreshWater<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|plot:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|range:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|isFreshWater:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0851}}<syntaxhighlight lang="lua">if (not Map.FindWater(plot, riverSourceRange, true)) then</syntaxhighlight>
{{CodeLine5|0852}}<syntaxhighlight lang="lua">if (not Map.FindWater(plot, seaWaterRange, false)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|FindWater]]
[[Category:Civ5 Terrain API|FindWater]]