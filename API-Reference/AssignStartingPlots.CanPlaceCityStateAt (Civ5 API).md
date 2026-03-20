{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' AssignStartingPlots:CanPlaceCityStateAt<b>(</b>'''int''' x, '''int''' y, {{Type5|AreaID}} area_ID, '''int''' force_it, '''int''' ignore_collisions<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|area_ID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|force_it:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ignore_collisions:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6399}}<syntaxhighlight lang="lua">if self:CanPlaceCityStateAt(x, y, iAreaID, force_it, ignore_collisions) == true then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6717}}<syntaxhighlight lang="lua">if self:CanPlaceCityStateAt(x, y, -1, false, false) == true then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanPlaceCityStateAt]]
[[Category:Civ5 Cities API|CanPlaceCityStateAt]]