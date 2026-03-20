{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


Determines continent for plot type.


=Usage=
<code>{{Type5|ArtStyleType}} Plot:GetContinentArtType<b>(</b><b>)</b></code>


'''Returned Value'''
:Returns number 0=Ocean, 1=America, 2=Asia, 3=Africa, 4=Europa


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local plot = Map.GetPlot(x, y);
if (plot:GetContinentArtType() == 1) then
print("America");</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0449}}<syntaxhighlight lang="lua">local continent = plot:GetContinentArtType();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetContinentArtType]]