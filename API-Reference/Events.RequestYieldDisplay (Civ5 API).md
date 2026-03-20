{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.RequestYieldDisplay<b>(</b>{{Type5|YieldDisplayType}} type, {{Type5|ResourceType}} arg1 = nil, {{Type5|ResourceType}} gridX = nil, '''int''' gridY = nil<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.RequestYieldDisplay.Add(''<function handler>'')</code> or invoke it directly through <code>Events.RequestYieldDisplay(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|type:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|gridX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|gridY:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0956}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay( YieldDisplayTypes.CITY_OWNED, pCity:GetX(), pCity:GetY() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0961}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay( YieldDisplayTypes.CITY_WORKED, pCity:GetX(), pCity:GetY() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1832}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay( YieldDisplayTypes.CITY_PURCHASABLE, pCity:GetX(), pCity:GetY() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0294}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay( YieldDisplayTypes.CITY_WORKED, lastCityEntered:GetX(), lastCityEntered:GetY() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0970}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay( YieldDisplayTypes.AREA, 2, gridX, gridY );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0995}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay( YieldDisplayTypes.EMPIRE );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0999}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay( YieldDisplayTypes.AREA, 2, unit:GetX(), unit:GetY() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1003}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay( YieldDisplayTypes.AREA, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0399}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay.Add( OnYieldDisplay );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceIconManager.lua}}
:<code>UI/InGame/ResourceIconManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0139}}<syntaxhighlight lang="lua">Events.RequestYieldDisplay.Add( OnRequestYieldDisplay );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RequestYieldDisplay]]
[[Category:Civ5 Yields API|RequestYieldDisplay]]