{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' City:IsNoOccupiedUnhappiness<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0215}}<syntaxhighlight lang="lua">if (city:IsOccupied() and not city:IsNoOccupiedUnhappiness()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0155}}<syntaxhighlight lang="lua">elseif(pCity:IsOccupied() and not pCity:IsNoOccupiedUnhappiness()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0695}}<syntaxhighlight lang="lua">if (pCity:IsOccupied() and not pCity:IsNoOccupiedUnhappiness()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2888}}<syntaxhighlight lang="lua">if (v:IsOccupied() and not v:IsNoOccupiedUnhappiness()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsNoOccupiedUnhappiness]]
[[Category:Civ5 Happiness API|IsNoOccupiedUnhappiness]]