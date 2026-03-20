{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("GameCalendarUtilities.lua")</code>
}}


=Usage=
<code>'''string''' GetShortDateString<b>(</b>'''int''' gameTurn, '''unknown''' calendarType, '''unknown''' gameSpeedType, '''int''' startYear<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|gameTurn:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|calendarType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|gameSpeedType:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|startYear:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0622}}<syntaxhighlight lang="lua">v:SetText(GetShortDateString(finalTurn, calendarType, gameSpeedType, startYear));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0628}}<syntaxhighlight lang="lua">v:SetText(GetShortDateString(turnIncrement, calendarType, gameSpeedType, startYear));</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetShortDateString]]