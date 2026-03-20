{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


On list provided by {{Type5|User:Sseckman}}, but no references yet found in scenario Lua files.


=Usage=
<code>'''void''' GameEvents.PlayerPreAIUnitUpdate<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Event Type'''
:Override: the first subscriber to return true will prevent the standard game mechanic to take place. Use it to replace the corresponding game mechanic with your own function.
::You can subscribe to this event through <code>GameEvents.PlayerPreAIUnitUpdate.Add(''<function handler>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''Presumably a player ID; as we don't know what the event relates to, the precise meaning of this parameter is also unclear.''
|}


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PlayerPreAIUnitUpdate]]
[[Category:Civ5 Units API|PlayerPreAIUnitUpdate]]
[[Category:Civ5 Players API|PlayerPreAIUnitUpdate]]