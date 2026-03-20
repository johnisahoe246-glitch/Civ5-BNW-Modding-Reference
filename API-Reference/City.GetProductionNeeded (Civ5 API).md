{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetProductionNeeded<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1523}}<syntaxhighlight lang="lua">local iProductionNeeded = pCity:GetProductionNeeded();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0599}}<syntaxhighlight lang="lua">local iProductionNeeded = city:GetProductionNeeded();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetProductionNeeded]]
[[Category:Civ5 City Production API|GetProductionNeeded]]