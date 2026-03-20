{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.EndTurnBlockingChanged<b>(</b>{{Type5|EndTurnBlockingType}} prevEndTurnBlockingType, {{Type5|EndTurnBlockingType}} newEndTurnBlockingType<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.EndTurnBlockingChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.EndTurnBlockingChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|prevEndTurnBlockingType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newEndTurnBlockingType:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0431}}<syntaxhighlight lang="lua">Events.EndTurnBlockingChanged.Add( OnEndTurnBlockingChanged );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|EndTurnBlockingChanged]]
[[Category:Civ5 Game Settings API|EndTurnBlockingChanged]]
[[Category:Civ5 Turns API|EndTurnBlockingChanged]]
[[Category:Civ5 Victory API|EndTurnBlockingChanged]]