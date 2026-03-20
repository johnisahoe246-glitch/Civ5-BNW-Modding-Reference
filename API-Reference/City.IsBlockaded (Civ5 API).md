{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' City:IsBlockaded<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0165}}<syntaxhighlight lang="lua">if (not city:IsCapital() and player:IsCapitalConnectedToCity(city) and not city:IsBlockaded()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0174}}<syntaxhighlight lang="lua">if (city:IsBlockaded()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0654}}<syntaxhighlight lang="lua">if (not isCapital and pPlayer:IsCapitalConnectedToCity(pCity) and not pCity:IsBlockaded()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0663}}<syntaxhighlight lang="lua">if (pCity:IsBlockaded()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsBlockaded]]