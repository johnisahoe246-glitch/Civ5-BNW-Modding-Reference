{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetNaturalWonderYieldModifier<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0420}}<syntaxhighlight lang="lua">local nwCulture = featureInfo.Culture * (100 + player:GetNaturalWonderYieldModifier())</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNaturalWonderYieldModifier]]
[[Category:Civ5 Features & Natural wonders API|GetNaturalWonderYieldModifier]]
[[Category:Civ5 Yields API|GetNaturalWonderYieldModifier]]
[[Category:Civ5 Buildings API|GetNaturalWonderYieldModifier]]