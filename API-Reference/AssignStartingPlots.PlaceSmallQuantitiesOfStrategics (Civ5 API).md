{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:PlaceSmallQuantitiesOfStrategics<b>(</b>'''int''' frequency, table('''int''' => '''int''') plot_list<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|frequency:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|plot_list:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1462}}<syntaxhighlight lang="lua">self:PlaceSmallQuantitiesOfStrategics(30, self.land_list);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|9713}}<syntaxhighlight lang="lua">self:PlaceSmallQuantitiesOfStrategics(23 * bonus_multiplier, self.land_list);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1429}}<syntaxhighlight lang="lua">self:PlaceSmallQuantitiesOfStrategics(32, self.land_list);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlaceSmallQuantitiesOfStrategics]]