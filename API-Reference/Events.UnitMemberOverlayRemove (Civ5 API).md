{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.UnitMemberOverlayRemove<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} unitID, '''int''' memberID<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.UnitMemberOverlayRemove.Add(''<function handler>'')</code> or invoke it directly through <code>Events.UnitMemberOverlayRemove(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|unitID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|memberID:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|UnitMemberOverlay.lua}}
:<code>UI/InGame/UnitMemberOverlay.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0289}}<syntaxhighlight lang="lua">Events.UnitMemberOverlayRemove.Add( OnUnitOverlayRemove );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitMemberOverlayRemove]]
[[Category:Civ5 Units API|UnitMemberOverlayRemove]]