{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.OpenInfoCorner<b>(</b>{{Type5|InfoCornerID}} infoType<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.OpenInfoCorner.Add(''<function handler>'')</code> or invoke it directly through <code>Events.OpenInfoCorner(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|infoType:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0042}}<syntaxhighlight lang="lua">Events.OpenInfoCorner( InfoCornerID.None );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0329}}<syntaxhighlight lang="lua">Events.OpenInfoCorner.Add( OnOpenInfoCorner );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoCorner.lua}}
:<code>UI/InGame/InfoCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0051}}<syntaxhighlight lang="lua">Events.OpenInfoCorner( iInfoType );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0088}}<syntaxhighlight lang="lua">Events.OpenInfoCorner( iWantInfoCorner );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPanel.lua}}
:<code>UI/InGame/TechPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0202}}<syntaxhighlight lang="lua">Events.OpenInfoCorner( InfoCornerID.Tech );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|OpenInfoCorner]]