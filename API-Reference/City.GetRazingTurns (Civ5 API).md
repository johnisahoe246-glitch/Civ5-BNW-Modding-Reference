{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetRazingTurns<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0184}}<syntaxhighlight lang="lua">controls.RazingIcon:SetToolTipString(Locale.ConvertTextKey( "TXT_KEY_CITY_BURNING", tostring(city:GetRazingTurns()) ));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0673}}<syntaxhighlight lang="lua">Controls.RazingIcon:LocalizeAndSetToolTip("TXT_KEY_CITY_BURNING", pCity:GetRazingTurns());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetRazingTurns]]