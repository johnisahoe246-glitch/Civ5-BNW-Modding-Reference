{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:CanBeThisNaturalWonderType<b>(</b>'''int''' x, '''int''' y, '''int''' wn, '''int''' rn<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|wn:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|rn:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5823}}<syntaxhighlight lang="lua">self:CanBeThisNaturalWonderType(x, y, nw_number, row_number)</syntaxhighlight>
{{CodeLine5|5824}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanBeThisNaturalWonderType]]
[[Category:Civ5 Features & Natural wonders API|CanBeThisNaturalWonderType]]
[[Category:Civ5 Buildings API|CanBeThisNaturalWonderType]]