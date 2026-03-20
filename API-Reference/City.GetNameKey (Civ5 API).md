{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' City:GetNameKey<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AnnexCityPopup.lua}}
:<code>UI/InGame/PopupsGeneric/AnnexCityPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0011}}<syntaxhighlight lang="lua">local cityNameKey = newCity:GetNameKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0145}}<syntaxhighlight lang="lua">local cityName = city:GetNameKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0702}}<syntaxhighlight lang="lua">local cityName = pCity:GetNameKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">cityName = Locale.ConvertTextKey( pCity:GetNameKey() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GreatPersonRewardPopup.lua}}
:<code>UI/InGame/Popups/GreatPersonRewardPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0024}}<syntaxhighlight lang="lua">Controls.DescriptionLabel:SetText(Locale.ConvertTextKey("TXT_KEY_GREAT_PERSON_REWARD", pGreatPersonInfo.Description, pCity:GetNameKey()));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LiberateMinorPopup.lua}}
:<code>UI/InGame/PopupsGeneric/LiberateMinorPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">local cityNameKey = pNewCity:GetNameKey();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNameKey]]