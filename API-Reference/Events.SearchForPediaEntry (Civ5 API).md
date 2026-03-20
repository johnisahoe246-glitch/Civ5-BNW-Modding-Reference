{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SearchForPediaEntry<b>(</b>'''string''' searchString<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SearchForPediaEntry.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SearchForPediaEntry(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|searchString:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvisorInfoPopup.lua}}
:<code>UI/InGame/Popups/AdvisorInfoPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0178}}<syntaxhighlight lang="lua">Events.SearchForPediaEntry( searchString );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6268}}<syntaxhighlight lang="lua">Events.SearchForPediaEntry.Add( SearchForPediaEntry );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0247}}<syntaxhighlight lang="lua">Events.SearchForPediaEntry("");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SearchForPediaEntry]]