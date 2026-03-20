{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.NaturalWonderRevealed<b>(</b>'''float''' i, '''int''' j<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.NaturalWonderRevealed.Add(''<function handler>'')</code> or invoke it directly through <code>Events.NaturalWonderRevealed(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|i:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|j:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2417}}<syntaxhighlight lang="lua">Events.NaturalWonderRevealed.Add( DiscoveredNaturalWonder );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|NaturalWonderRevealed]]
[[Category:Civ5 Features & Natural wonders API|NaturalWonderRevealed]]
[[Category:Civ5 Fog API|NaturalWonderRevealed]]
[[Category:Civ5 Buildings API|NaturalWonderRevealed]]