{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendReturnCivilian<b>(</b>'''bool''' arg0, '''int''' giftedPlayer, {{Type5|UnitID}} unitIndex<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|giftedPlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitIndex:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ReturnCivilianPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ReturnCivilianPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0047}}<syntaxhighlight lang="lua">Network.SendReturnCivilian(true, iGiftedPlayer, iUnitIndex);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">Network.SendReturnCivilian(false, iGiftedPlayer, iUnitIndex);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendReturnCivilian]]