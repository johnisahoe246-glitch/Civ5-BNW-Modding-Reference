{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Unit:HasName<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0275}}<syntaxhighlight lang="lua">if(unit:HasName()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0169}}<syntaxhighlight lang="lua">if(pUnit:HasName()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1584}}<syntaxhighlight lang="lua">if (pUnit:HasName()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|HasName]]