{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' AssignStartingPlots:AttemptToPlaceNaturalWonder<b>(</b>'''int''' wonder_number, '''int''' row_number<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|wonder_number:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|row_number:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6054}}<syntaxhighlight lang="lua">local bSuccess = self:AttemptToPlaceNaturalWonder(nw_number, row_number)</syntaxhighlight>
{{CodeLine5|6055}}<syntaxhighlight lang="lua">if bSuccess then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AttemptToPlaceNaturalWonder]]
[[Category:Civ5 Features & Natural wonders API|AttemptToPlaceNaturalWonder]]
[[Category:Civ5 Buildings API|AttemptToPlaceNaturalWonder]]