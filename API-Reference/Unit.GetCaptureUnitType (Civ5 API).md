{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|UnitType}} Unit:GetCaptureUnitType<b>(</b>{{Type5|CivilizationType}} civilization<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|civilization:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ReturnCivilianPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ReturnCivilianPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">local iNewUnit = pUnit:GetCaptureUnitType(pGiftingPlayer:GetCivilizationType());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCaptureUnitType]]
[[Category:Civ5 Units API|GetCaptureUnitType]]
[[Category:Civ5 Combat API|GetCaptureUnitType]]