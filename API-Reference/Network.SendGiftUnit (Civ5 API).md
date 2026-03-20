{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendGiftUnit<b>(</b>'''int''' giftedPlayer, {{Type5|UnitID}} unitIndex<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|giftedPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitIndex:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ConfirmGiftPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ConfirmGiftPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0035}}<syntaxhighlight lang="lua">Network.SendGiftUnit(iGiftedPlayer, iUnitIndex);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendGiftUnit]]
[[Category:Civ5 Units API|SendGiftUnit]]
[[Category:Civ5 Diplomacy API|SendGiftUnit]]
[[Category:Civ5 City States API|SendGiftUnit]]