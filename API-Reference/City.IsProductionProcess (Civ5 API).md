{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:IsProductionProcess<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0268}}<syntaxhighlight lang="lua">if (city:IsProduction() and not city:IsProductionProcess()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1524}}<syntaxhighlight lang="lua">if (pCity:IsProductionProcess()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1569}}<syntaxhighlight lang="lua">local bGeneratingProduction = pCity:IsProductionProcess() or pCity:GetCurrentProductionDifferenceTimes100(false, false) == 0;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1604}}<syntaxhighlight lang="lua">if (not pCity:IsProductionProcess()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0600}}<syntaxhighlight lang="lua">if (city:IsProductionProcess()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0632}}<syntaxhighlight lang="lua">local bGeneratingProduction = city:IsProductionProcess() or city:GetCurrentProductionDifferenceTimes100(false, false) == 0;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsProductionProcess]]
[[Category:Civ5 City Production API|IsProductionProcess]]