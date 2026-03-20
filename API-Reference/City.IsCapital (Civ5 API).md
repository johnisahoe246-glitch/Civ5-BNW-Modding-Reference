{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:IsCapital<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0150}}<syntaxhighlight lang="lua">local isCapital = city:IsCapital() or Players[city:GetOriginalOwner()]:IsMinorCiv();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">if (city:IsCapital() and not player:IsMinorCiv()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0165}}<syntaxhighlight lang="lua">if (not city:IsCapital() and player:IsCapitalConnectedToCity(city) and not city:IsBlockaded()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0149}}<syntaxhighlight lang="lua">if(pCity:IsCapital())then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0649}}<syntaxhighlight lang="lua">local isCapital = pCity:IsCapital();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0302}}<syntaxhighlight lang="lua">if (not pCity:IsCapital()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsCapital]]
[[Category:Civ5 Cities API|IsCapital]]