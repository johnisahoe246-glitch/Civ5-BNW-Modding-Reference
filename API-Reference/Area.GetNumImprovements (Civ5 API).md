{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Area}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Area:GetNumImprovements<b>(</b>{{Type5|ImprovementType}} improvement<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|improvement:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MapGenerator.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/MapGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0699}}<syntaxhighlight lang="lua">local improvementCount = area:GetNumImprovements(improvementID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumImprovements]]
[[Category:Civ5 Improvements API|GetNumImprovements]]