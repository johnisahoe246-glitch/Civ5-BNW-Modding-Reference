{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.OpenPlayerDealScreenEvent<b>(</b>{{Type5|PlayerID}} player, '''int''' target = nil<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.OpenPlayerDealScreenEvent.Add(''<function handler>'')</code> or invoke it directly through <code>Events.OpenPlayerDealScreenEvent(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|target:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1078}}<syntaxhighlight lang="lua">Events.OpenPlayerDealScreenEvent( ePlayer );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0286}}<syntaxhighlight lang="lua">Events.OpenPlayerDealScreenEvent.Add( OnOpenPlayerDealScreen );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0326}}<syntaxhighlight lang="lua">Events.OpenPlayerDealScreenEvent(ePlayer);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|OpenPlayerDealScreenEvent]]
[[Category:Civ5 Players API|OpenPlayerDealScreenEvent]]
[[Category:Civ5 Diplomacy API|OpenPlayerDealScreenEvent]]
[[Category:Civ5 Trade API|OpenPlayerDealScreenEvent]]