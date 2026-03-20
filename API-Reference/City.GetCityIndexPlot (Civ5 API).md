{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|Plot}} City:GetCityIndexPlot<b>(</b>{{Type5|CityPlotID}} index<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|index:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1695}}<syntaxhighlight lang="lua">local plot = pHeadSelectedCity:GetCityIndexPlot( iPlotIndex );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1721}}<syntaxhighlight lang="lua">local plot = pCity:GetCityIndexPlot( i );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCityIndexPlot]]
[[Category:Civ5 Cities API|GetCityIndexPlot]]