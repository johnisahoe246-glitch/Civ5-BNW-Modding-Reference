{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetNumCityPlots<b>(</b><b>)</b></code>


'''Returned Value'''
:The number of plots that are owned by the city.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1720}}<syntaxhighlight lang="lua">for i = 0, pCity:GetNumCityPlots() - 1, 1 do</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumCityPlots]]
[[Category:Civ5 Cities API|GetNumCityPlots]]