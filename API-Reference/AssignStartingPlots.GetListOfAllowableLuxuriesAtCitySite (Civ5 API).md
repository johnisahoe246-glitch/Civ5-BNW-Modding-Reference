{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''' AssignStartingPlots:GetListOfAllowableLuxuriesAtCitySite<b>(</b>'''int''' x, '''int''' y, '''int''' radius<b>)</b></code>


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
|valign="top" style="padding-right:6px;"|radius:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|8640}}<syntaxhighlight lang="lua">local allowed_luxuries = self:GetListOfAllowableLuxuriesAtCitySite(x, y, 2)</syntaxhighlight>
{{CodeLine5|8641}}<syntaxhighlight lang="lua">--print("-"); print("--- Eligible Types List for Second Luxury in Region#", region_number, "---");</syntaxhighlight>
{{CodeLine5|8642}}<syntaxhighlight lang="lua">-- See if any Random types are eligible.</syntaxhighlight>
{{CodeLine5|8643}}<syntaxhighlight lang="lua">for loop, res_ID in ipairs(self.resourceIDs_assigned_to_random) do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|8607}}<syntaxhighlight lang="lua">local allowed_luxuries = self:GetListOfAllowableLuxuriesAtCitySite(x, y, 2)</syntaxhighlight>
{{CodeLine5|8608}}<syntaxhighlight lang="lua">local lux_possible_for_cs = {}; -- Recorded with ID as key, weighting as data entry</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8816}}<syntaxhighlight lang="lua">local allowed_luxuries = self:GetListOfAllowableLuxuriesAtCitySite(x, y, 2)</syntaxhighlight>
{{CodeLine5|8817}}<syntaxhighlight lang="lua">print("-"); print("--- Eligible Types List for Second Luxury in Region#", region_number, "---");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetListOfAllowableLuxuriesAtCitySite]]
[[Category:Civ5 Cities API|GetListOfAllowableLuxuriesAtCitySite]]