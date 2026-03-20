{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:IsPuppet<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0198}}<syntaxhighlight lang="lua">if (city:IsPuppet()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1184}}<syntaxhighlight lang="lua">if city and not city:IsPuppet() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0152}}<syntaxhighlight lang="lua">elseif(pCity:IsPuppet()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0421}}<syntaxhighlight lang="lua">if (not city:IsPuppet()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0687}}<syntaxhighlight lang="lua">if (pCity:IsPuppet()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0760}}<syntaxhighlight lang="lua">if city and city:IsPuppet() then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsPuppet]]
[[Category:Civ5 Cities API|IsPuppet]]