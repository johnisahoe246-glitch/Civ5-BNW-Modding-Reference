{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.RequestRefreshAdditionalInformationDropdownEntries<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.RequestRefreshAdditionalInformationDropdownEntries.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.RequestRefreshAdditionalInformationDropdownEntries(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">LuaEvents.RequestRefreshAdditionalInformationDropdownEntries.Add(RefreshAdditionalInformationEntries);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0229}}<syntaxhighlight lang="lua">LuaEvents.RequestRefreshAdditionalInformationDropdownEntries();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RequestRefreshAdditionalInformationDropdownEntries]]