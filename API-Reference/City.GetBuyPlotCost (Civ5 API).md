{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetBuyPlotCost<b>(</b>'''int''' x, '''int''' y<b>)</b></code>


'''Returned Value'''
:No description available.
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

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1841}}<syntaxhighlight lang="lua">local iPlotCost = pCity:GetBuyPlotCost( plot:GetX(), plot:GetY() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2141}}<syntaxhighlight lang="lua">local iPlotCost = city:GetBuyPlotCost( hexX, hexY );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetBuyPlotCost]]