{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


Presumably called when players meet, but referring to teams. Sample usages have not been found.


=Usage=
<code>'''void''' GameEvents.TeamMeet<b>(</b>'''unknown''' playeractive, '''unknown''' playermet<b>)</b></code>


'''Event Type'''
:Override: the first subscriber to return true will prevent the standard game mechanic to take place. Use it to replace the corresponding game mechanic with your own function.
::You can subscribe to this event through <code>GameEvents.TeamMeet.Add(''<function handler>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|playeractive:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|playermet:
|valign="top"| ''No description available.''
|}


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|TeamMeet]]
[[Category:Civ5 Diplomacy API|TeamMeet]]