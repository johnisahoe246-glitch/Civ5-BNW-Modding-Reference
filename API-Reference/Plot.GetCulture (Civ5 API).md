{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
<br/>
This method was removed in Gods & Kings.
}}


Determines the amount of culture yielded by working the plot.


=Usage=
<code>'''int''' Plot:GetCulture<b>(</b><b>)</b></code>


'''Returned Value'''
:The amount of culture yielded by working the plot.


=Source code samples=
{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0410}}<syntaxhighlight lang="lua">local iNumCulture = plot:GetCulture();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|YieldIconManager.lua}}
:<code>UI/InGame/YieldIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0222}}<syntaxhighlight lang="lua">local iCulture    = plot:GetCulture();-- + math.random( 0, 13 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCulture]]
[[Category:Civ5 Culture API|GetCulture]]