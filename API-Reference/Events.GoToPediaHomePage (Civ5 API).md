{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.GoToPediaHomePage<b>(</b>{{Type5|ImprovementType}} homePage<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.GoToPediaHomePage.Add(''<function handler>'')</code> or invoke it directly through <code>Events.GoToPediaHomePage(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|homePage:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvisorInfoPopup.lua}}
:<code>UI/InGame/Popups/AdvisorInfoPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0187}}<syntaxhighlight lang="lua">Events.GoToPediaHomePage( GameInfo.Concepts[g_strConcept].CivilopediaPage );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6279}}<syntaxhighlight lang="lua">Events.GoToPediaHomePage.Add( GoToPediaHomePage );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GoToPediaHomePage]]