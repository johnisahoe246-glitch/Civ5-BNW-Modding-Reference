{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.EndTurnTimerUpdate<b>(</b>'''int''' percentComplete<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.EndTurnTimerUpdate.Add(''<function handler>'')</code> or invoke it directly through <code>Events.EndTurnTimerUpdate(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|percentComplete:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0444}}<syntaxhighlight lang="lua">Events.EndTurnTimerUpdate.Add(OnEndTurnTimerUpdate);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|EndTurnTimerUpdate]]
[[Category:Civ5 Game Settings API|EndTurnTimerUpdate]]
[[Category:Civ5 Turns API|EndTurnTimerUpdate]]
[[Category:Civ5 Victory API|EndTurnTimerUpdate]]