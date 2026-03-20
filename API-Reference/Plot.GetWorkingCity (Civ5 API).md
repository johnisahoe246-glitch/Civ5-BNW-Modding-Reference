{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|City}} Plot:GetWorkingCity<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1769}}<syntaxhighlight lang="lua">elseif ( plot:GetWorkingCity():GetID() ~= pCity:GetID() and  plot:GetWorkingCity():IsWorkingPlot( plot ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1805}}<syntaxhighlight lang="lua">elseif ( pCity:CanWork( plot ) or plot:GetWorkingCity():GetID() ~= pCity:GetID() ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetWorkingCity]]
[[Category:Civ5 Cities API|GetWorkingCity]]