{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendCityBuyPlot<b>(</b>{{Type5|CityID}} arg0, '''int''' plotX, '''int''' plotY<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|plotX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|plotY:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1698}}<syntaxhighlight lang="lua">Network.SendCityBuyPlot(pHeadSelectedCity:GetID(), plotX, plotY);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendCityBuyPlot]]
[[Category:Civ5 Cities API|SendCityBuyPlot]]