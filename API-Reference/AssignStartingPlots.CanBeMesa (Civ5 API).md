{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:CanBeMesa<b>(</b>'''int''' x, '''int''' y<b>)</b></code>


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
{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5337}}<syntaxhighlight lang="lua">self:CanBeMesa(x, y)</syntaxhighlight>
{{CodeLine5|5338}}<syntaxhighlight lang="lua">self:CanBeReef(x, y)</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Great_Plains_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1256}}<syntaxhighlight lang="lua">self:CanBeMesa(x, y)</syntaxhighlight>
{{CodeLine5|1257}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanBeMesa]]