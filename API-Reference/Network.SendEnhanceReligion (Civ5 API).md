{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendEnhanceReligion<b>(</b>{{Type5|PlayerID}} arg0, {{Type5|ReligionType}} CurrentReligion, '''unknown''' customName, '''unknown''' arg3, '''int''' arg4, '''int''' cityX, '''int''' cityY<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|CurrentReligion:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|customName:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg3:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg4:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|cityX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|cityY:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0595}}<syntaxhighlight lang="lua">Network.SendEnhanceReligion(Game.GetActivePlayer(), g_CurrentReligionID, customName, g_Beliefs[4], g_Beliefs[5], g_iCityX, g_iCityY);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendEnhanceReligion]]
[[Category:Civ5 Religion API|SendEnhanceReligion]]