{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.EndGameShow<b>(</b>{{Type5|EndGameType}} type, {{Type5|TeamID}} team<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.EndGameShow.Add(''<function handler>'')</code> or invoke it directly through <code>Events.EndGameShow(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|type:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|team:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0404}}<syntaxhighlight lang="lua">if( which == 1 ) then Events.EndGameShow( EndGameTypes.Technology, Game.GetActivePlayer() );</syntaxhighlight>
{{CodeLine5|0405}}<syntaxhighlight lang="lua">elseif( which == 2 ) then Events.EndGameShow( EndGameTypes.Domination, Game.GetActivePlayer() );</syntaxhighlight>
{{CodeLine5|0406}}<syntaxhighlight lang="lua">elseif( which == 3 ) then Events.EndGameShow( EndGameTypes.Culture, Game.GetActivePlayer() );</syntaxhighlight>
{{CodeLine5|0407}}<syntaxhighlight lang="lua">elseif( which == 4 ) then Events.EndGameShow( EndGameTypes.Diplomatic, Game.GetActivePlayer() );</syntaxhighlight>
{{CodeLine5|0408}}<syntaxhighlight lang="lua">elseif( which == 5 ) then Events.EndGameShow( EndGameTypes.Time, Game.GetActivePlayer() );</syntaxhighlight>
{{CodeLine5|0409}}<syntaxhighlight lang="lua">elseif( which == 6 ) then Events.EndGameShow( EndGameTypes.Time, Game.GetActivePlayer() + 1 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0215}}<syntaxhighlight lang="lua">Events.EndGameShow.Add( OnDisplay );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|EndGameShow]]