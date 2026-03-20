{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' Player:GetCivilizationAdjective<b>(</b>'''int''' form<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|form:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|MinorCivEnterTerritoryPopup.lua}}
:<code>UI/InGame/PopupsGeneric/MinorCivEnterTerritoryPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0014}}<syntaxhighlight lang="lua">popupText = Locale.ConvertTextKey("TXT_KEY_POPUP_ENTER_MINOR_CIV_LANDS", Players[plot:GetOwner()]:GetCivilizationAdjective());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1290}}<syntaxhighlight lang="lua">CivAdjective = player:GetCivilizationAdjective(),</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCivilizationAdjective]]
[[Category:Civ5 Players API|GetCivilizationAdjective]]