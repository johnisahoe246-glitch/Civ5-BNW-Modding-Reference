{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.WorldMouseOver<b>(</b>'''int''' worldHasMouseOver<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.WorldMouseOver.Add(''<function handler>'')</code> or invoke it directly through <code>Events.WorldMouseOver(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|worldHasMouseOver:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1774}}<syntaxhighlight lang="lua">Events.WorldMouseOver.Add( OnWorldMouseOver );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpManager.lua}}
:<code>UI/InGame/PlotHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0353}}<syntaxhighlight lang="lua">Controls.TheBox:RegisterCallback( Mouse.eMouseEnter, function() Events.WorldMouseOver( true  ); end );</syntaxhighlight>
{{CodeLine5|0354}}<syntaxhighlight lang="lua">Controls.TheBox:RegisterCallback( Mouse.eMouseExit,  function() Events.WorldMouseOver( false ); end );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|WorldMouseOver]]