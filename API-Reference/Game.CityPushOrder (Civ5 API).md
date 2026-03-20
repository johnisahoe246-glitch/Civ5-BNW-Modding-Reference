{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.CityPushOrder<b>(</b>{{Type5|City}} city, {{Type5|OrderType}} order, {{Type5|UnitType}} data, '''bool''' alt, '''bool''' shift, '''bool''' ctrl<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|city:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|order:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|data:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|alt:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|shift:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ctrl:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">Game.CityPushOrder(city, eOrder, iData, false, not g_append, true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CityPushOrder]]
[[Category:Civ5 Cities API|CityPushOrder]]