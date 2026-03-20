{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.GameplaySetActivePlayer<b>(</b>{{Type5|PlayerID}} activePlayer, '''int''' prevActivePlayer<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.GameplaySetActivePlayer.Add(''<function handler>'')</code> or invoke it directly through <code>Events.GameplaySetActivePlayer(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|activePlayer:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|prevActivePlayer:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0454}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add( OnPlayerChangedEvent );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorCounselPopup.lua}}
:<code>UI/InGame/Popups/AdvisorCounselPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0317}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(Close);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AnnexCityPopup.lua}}
:<code>UI/InGame/PopupsGeneric/AnnexCityPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(HideWindow);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|BarbarianCampPopup.lua}}
:<code>UI/InGame/Popups/BarbarianCampPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0065}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnCloseButtonClicked);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseFaithGreatPerson.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseFaithGreatPerson.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0188}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnActivePlayerChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1233}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnCityBannerActivePlayerChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add( OnChangeEvent );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2412}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnEventActivePlayerChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6455}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnClose);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0540}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnBack);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0444}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnDiploCornerActivePlayerChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0632}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnDiploListActivePlayerChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0523}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnGameMenuActivePlayerChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoCorner.lua}}
:<code>UI/InGame/InfoCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0094}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnInfoCornerActivePlayerChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0385}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnMPListActivePlayerChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0355}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnNotificationPanelActivePlayerChanged);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0407}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnNotificationsActivePlayerChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCityName.lua}}
:<code>UI/InGame/Popups/SetCityName.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0135}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnCancel);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SimpleDiploTrade.lua}}
:<code>UI/InGame/WorldView/SimpleDiploTrade.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0021}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnDiploActivePlayerChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechAwardPopup.lua}}
:<code>UI/InGame/Popups/TechAwardPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0156}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnTechAwardActivePlayerChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPanel.lua}}
:<code>UI/InGame/TechPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0223}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnTechPanelActivePlayerChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0817}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnTechTreeActivePlayerChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0090}}<syntaxhighlight lang="lua">Events.GameplaySetActivePlayer.Add(OnChangeEvent);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GameplaySetActivePlayer]]
[[Category:Civ5 Players API|GameplaySetActivePlayer]]