{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.UnitGarrison<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' garrisoned<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.UnitGarrison.Add(''<function handler>'')</code> or invoke it directly through <code>Events.UnitGarrison(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|garrisoned:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1155}}<syntaxhighlight lang="lua">Events.UnitGarrison.Add( OnUnitGarrison );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0799}}<syntaxhighlight lang="lua">Events.UnitGarrison.Add( OnDirty );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0952}}<syntaxhighlight lang="lua">Events.UnitGarrison.Add( OnFlagTypeChange );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0085}}<syntaxhighlight lang="lua">Events.UnitGarrison.Add( OnChangeEvent );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitGarrison]]
[[Category:Civ5 Units API|UnitGarrison]]
[[Category:Civ5 Combat API|UnitGarrison]]