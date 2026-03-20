{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.AdditionalInformationDropdownSortEntries<b>(</b>table('''int''' => '''table''') entries<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.AdditionalInformationDropdownSortEntries.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.AdditionalInformationDropdownSortEntries(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|entries:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0048}}<syntaxhighlight lang="lua">LuaEvents.AdditionalInformationDropdownSortEntries(additionalEntries);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0084}}<syntaxhighlight lang="lua">LuaEvents.AdditionalInformationDropdownSortEntries.Add(SortAdditionalInformationDropdownEntries);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AdditionalInformationDropdownSortEntries]]