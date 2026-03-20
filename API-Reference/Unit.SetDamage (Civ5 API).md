{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Unit:SetDamage<b>(</b>'''int''' newValue, {{Type5|PlayerID}} player, '''bool''' notifyEntity = true<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|newValue:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|notifyEntity:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0210}}<syntaxhighlight lang="lua">pNewUnit:SetDamage(iUnitDamage);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetDamage]]
[[Category:Civ5 Combat API|SetDamage]]