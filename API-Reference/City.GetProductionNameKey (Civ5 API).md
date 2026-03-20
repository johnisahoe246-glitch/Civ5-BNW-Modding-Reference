{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' City:GetProductionNameKey<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0321}}<syntaxhighlight lang="lua">local cityProductionName = city:GetProductionNameKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0126}}<syntaxhighlight lang="lua">sortEntry.Production = pCity:GetProductionNameKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0839}}<syntaxhighlight lang="lua">local szItemName = Locale.ConvertTextKey(pCity:GetProductionNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1605}}<syntaxhighlight lang="lua">strToolTip = strToolTip .. Locale.ConvertTextKey("TXT_KEY_PRODUCTION_HELP_TEXT", pCity:GetProductionNameKey(), strNumTurns);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0505}}<syntaxhighlight lang="lua">strItemName = Locale.ConvertTextKey(city:GetProductionNameKey());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetProductionNameKey]]
[[Category:Civ5 City Production API|GetProductionNameKey]]