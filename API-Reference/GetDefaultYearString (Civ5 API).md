{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a global function. Use: <code>include("GameCalendarUtilities.lua")</code>
}}


=Usage=
<code>'''string''' GetDefaultYearString<b>(</b>'''int''' year<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|year:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|GameCalendarUtilities.lua}}
:<code>Gameplay/Lua/GameCalendarUtilities.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0062}}<syntaxhighlight lang="lua">local yearString = GetDefaultYearString(turnYear);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0072}}<syntaxhighlight lang="lua">return GetDefaultYearString(turnYear);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetDefaultYearString]]