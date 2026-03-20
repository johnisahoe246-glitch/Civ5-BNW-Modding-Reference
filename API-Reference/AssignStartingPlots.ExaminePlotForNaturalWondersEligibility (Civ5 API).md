{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' AssignStartingPlots:ExaminePlotForNaturalWondersEligibility<b>(</b>'''int''' x, '''int''' y<b>)</b></code>


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
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5186}}<syntaxhighlight lang="lua">if self:ExaminePlotForNaturalWondersEligibility(x, y) == false then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5200}}<syntaxhighlight lang="lua">if self:ExaminePlotForNaturalWondersEligibility(adjX, adjY) == false then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ExaminePlotForNaturalWondersEligibility]]
[[Category:Civ5 Features & Natural wonders API|ExaminePlotForNaturalWondersEligibility]]
[[Category:Civ5 Buildings API|ExaminePlotForNaturalWondersEligibility]]