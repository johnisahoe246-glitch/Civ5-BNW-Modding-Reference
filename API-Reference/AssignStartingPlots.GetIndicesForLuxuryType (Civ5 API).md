{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''', '''int''', '''int''', '''int''' AssignStartingPlots:GetIndicesForLuxuryType<b>(</b>{{Type5|ResourceType}} resource_<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|resource_:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|8526}}<syntaxhighlight lang="lua">primary, secondary, tertiary, quaternary = self:GetIndicesForLuxuryType(this_region_luxury);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8575}}<syntaxhighlight lang="lua">primary, secondary, tertiary, quaternary = self:GetIndicesForLuxuryType(random_res);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8676}}<syntaxhighlight lang="lua">primary, secondary, tertiary, quaternary = self:GetIndicesForLuxuryType(use_this_ID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|8705}}<syntaxhighlight lang="lua">primary, secondary, tertiary, quaternary = self:GetIndicesForLuxuryType(res_ID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetIndicesForLuxuryType]]