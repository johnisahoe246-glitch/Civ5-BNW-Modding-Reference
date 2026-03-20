{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventRawResourceIconCreated<b>(</b>'''float''' hexPosX, '''int''' hexPosY, '''unknown''' ImprovementType, {{Type5|ResourceType}} ResourceType<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventRawResourceIconCreated.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventRawResourceIconCreated(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|hexPosX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|hexPosY:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ImprovementType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ResourceType:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ResourceIconManager.lua}}
:<code>UI/InGame/ResourceIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">Events.SerialEventRawResourceIconCreated.Add( OnResourceAdded )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0127}}<syntaxhighlight lang="lua">function OnRequestYieldDisplay( type )</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventRawResourceIconCreated]]
[[Category:Civ5 Resources API|SerialEventRawResourceIconCreated]]