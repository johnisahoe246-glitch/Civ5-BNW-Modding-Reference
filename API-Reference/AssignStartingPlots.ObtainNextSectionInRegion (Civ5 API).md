{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>table('''int''' => '''int'''), table('''int''' => '''int'''), '''unknown''', '''unknown''', '''unknown''', '''unknown''', '''unknown''' AssignStartingPlots:ObtainNextSectionInRegion<b>(</b>'''int''' incoming_west_x, '''int''' incoming_south_y, '''int''' incoming_width, '''int''' incoming_height, {{Type5|AreaID}} areaID, '''int''' force_it, '''int''' ignore_collisions<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|incoming_west_x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|incoming_south_y:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|incoming_width:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|incoming_height:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|areaID:
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
{{CodeLine5|6517}}<syntaxhighlight lang="lua">reached_middle = self:ObtainNextSectionInRegion(curWX, curSY, curWid, curHei, iAreaID, false, false) -- Don't force it. Yet.</syntaxhighlight>
{{CodeLine5|6518}}<syntaxhighlight lang="lua">curWX, curSY, curWid, curHei = nextWX, nextSY, nextWid, nextHei;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ObtainNextSectionInRegion]]