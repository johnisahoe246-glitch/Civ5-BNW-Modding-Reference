{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.ProductionPopup<b>(</b>'''bool''' isHide<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.ProductionPopup.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.ProductionPopup(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|isHide:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2342}}<syntaxhighlight lang="lua">LuaEvents.ProductionPopup.Add( OnProductionPopup );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1102}}<syntaxhighlight lang="lua">LuaEvents.ProductionPopup( bIsHide );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ProductionPopup]]
[[Category:Civ5 City Production API|ProductionPopup]]