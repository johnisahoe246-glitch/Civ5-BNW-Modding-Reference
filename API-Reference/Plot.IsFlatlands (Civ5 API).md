{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:IsFlatlands<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Amazon_XP.lua (G&K)}}
:<code>DLC/Expansion/Maps/Amazon_XP.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0405}}<syntaxhighlight lang="lua">elseif plot:IsFlatlands() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0413}}<syntaxhighlight lang="lua">if plot:IsFlatlands() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Great_Plains.lua}}
:<code>Maps/Great_Plains.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0536}}<syntaxhighlight lang="lua">if (long < 0.16 and lat > 0.23) and (plot:IsFlatlands() or plot:IsHills()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Ring.lua}}
:<code>Maps/Ring.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0530}}<syntaxhighlight lang="lua">if plot:IsFlatlands() or plot:IsHills() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Skirmish.lua}}
:<code>Maps/Skirmish.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0237}}<syntaxhighlight lang="lua">if plot:IsFlatlands() then -- Check for adjacent Mountain plot; if found, change this plot to Hills.</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsFlatlands]]