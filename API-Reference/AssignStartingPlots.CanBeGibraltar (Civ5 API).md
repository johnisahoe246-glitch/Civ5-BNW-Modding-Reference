{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:CanBeGibraltar<b>(</b>'''int''' x, '''int''' y<b>)</b></code>


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

{{PseudoH4|AssignStartingPlots.lua}}
:<code>Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|5335}}<syntaxhighlight lang="lua">self:CanBeGibraltar(x, y)</syntaxhighlight>
{{CodeLine5|5336}}<syntaxhighlight lang="lua">self:CanBeFuji(x, y)</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Europe.lua (G&K)}}
:<code>DLC/Expansion/Maps/Europe.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1056}}<syntaxhighlight lang="lua">self:CanBeGibraltar(x, y)</syntaxhighlight>
{{CodeLine5|1057}}<syntaxhighlight lang="lua">self:CanBeMtSinai(x, y)</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanBeGibraltar]]