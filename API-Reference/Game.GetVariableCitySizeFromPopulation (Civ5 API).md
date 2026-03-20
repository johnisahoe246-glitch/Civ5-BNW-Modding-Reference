{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.GetVariableCitySizeFromPopulation<b>(</b>'''int''' population<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|population:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0166}}<syntaxhighlight lang="lua">local iCitySize = Game.GetVariableCitySizeFromPopulation( g_iPopulation );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetVariableCitySizeFromPopulation]]
[[Category:Civ5 Cities API|GetVariableCitySizeFromPopulation]]
[[Category:Civ5 Food & Population API|GetVariableCitySizeFromPopulation]]