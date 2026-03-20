{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|Area}} Plot:Area<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|WorldBuilderRandomItems.lua}}
:<code>Gameplay/Lua/WorldBuilderRandomItems.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0050}}<syntaxhighlight lang="lua">local area = plot:Area();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0086}}<syntaxhighlight lang="lua">local otherArea = otherPlot:Area();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0168}}<syntaxhighlight lang="lua">if (bestArea:GetID() == plot:Area():GetID() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0182}}<syntaxhighlight lang="lua">if (otherPlot ~= nil and (otherPlot:Area():GetID() == bestArea:GetID() )) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Area]]
[[Category:Civ5 Terrain API|Area]]