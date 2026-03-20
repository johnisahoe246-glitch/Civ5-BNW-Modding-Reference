{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.UnitEmbark<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.UnitEmbark.Add(''<function handler>'')</code> or invoke it directly through <code>Events.UnitEmbark(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitID:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0800}}<syntaxhighlight lang="lua">Events.UnitEmbark.Add( OnDirty );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0953}}<syntaxhighlight lang="lua">Events.UnitEmbark.Add( OnFlagTypeChange );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0086}}<syntaxhighlight lang="lua">Events.UnitEmbark.Add( OnChangeEvent );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitEmbark]]
[[Category:Civ5 Units API|UnitEmbark]]
[[Category:Civ5 Movement API|UnitEmbark]]