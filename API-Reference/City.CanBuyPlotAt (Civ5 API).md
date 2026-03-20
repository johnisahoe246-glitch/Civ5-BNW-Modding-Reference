{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' City:CanBuyPlotAt<b>(</b>'''int''' hexX, '''int''' hexY, '''bool''' arg2<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|hexX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|hexY:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1838}}<syntaxhighlight lang="lua">if (pCity:CanBuyPlotAt(plot:GetX(), plot:GetY(), false)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1848}}<syntaxhighlight lang="lua">elseif (pCity:CanBuyPlotAt(plot:GetX(), plot:GetY(), true)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2140}}<syntaxhighlight lang="lua">if (city:CanBuyPlotAt( hexX, hexY, true)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanBuyPlotAt]]