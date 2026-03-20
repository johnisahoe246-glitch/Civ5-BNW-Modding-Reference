{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ButtonBase''', {{Type5|EditBox}}, {{Type5|Grid}}, {{Type5|GridButton}}, {{Type5|Image}}, {{Type5|Slider}} and {{Type5|TextButton}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetVoid1<b>(</b>{{Type5|OrderType}} MAINTAIN_GOLD<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|MAINTAIN_GOLD:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Too many occurences. Only 50 out of 347 are listed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0589}}<syntaxhighlight lang="lua">instance.Button:SetVoid1( -1 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0598}}<syntaxhighlight lang="lua">controlTable.BannerButton:SetVoid1( gridPosX );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0611}}<syntaxhighlight lang="lua">controlTable.CityRangeStrikeButton:SetVoid1(playerID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0617}}<syntaxhighlight lang="lua">svStrikeButton.CityRangeStrikeButton:SetVoid1(playerID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">Controls.SortPopulation:SetVoid1( ePopulation );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0528}}<syntaxhighlight lang="lua">controlTable.BuildingButton:SetVoid1( buildingID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1917}}<syntaxhighlight lang="lua">Controls.b2remove:SetVoid1( 1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1919}}<syntaxhighlight lang="lua">Controls.b3remove:SetVoid1( 2 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1921}}<syntaxhighlight lang="lua">Controls.b4remove:SetVoid1( 3 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1923}}<syntaxhighlight lang="lua">Controls.b5remove:SetVoid1( 4 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1934}}<syntaxhighlight lang="lua">Controls.b1down:SetVoid1( 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1957}}<syntaxhighlight lang="lua">Controls.b6up:SetVoid1( 4 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2268}}<syntaxhighlight lang="lua">Controls.BalancedFocusButton:SetVoid1( CityAIFocusTypes.NO_CITY_AI_FOCUS_TYPE )</syntaxhighlight>
{{CodeLine5|2269}}<syntaxhighlight lang="lua">Controls.BalancedFocusButton:RegisterCallback( Mouse.eLClick, FocusChanged );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2277}}<syntaxhighlight lang="lua">Controls.GoldFocusButton:SetVoid1( CityAIFocusTypes.CITY_AI_FOCUS_TYPE_GOLD )</syntaxhighlight>
{{CodeLine5|2278}}<syntaxhighlight lang="lua">Controls.GoldFocusButton:RegisterCallback( Mouse.eLClick, FocusChanged );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">Controls.CurrentDealsButton:SetVoid1( 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">controlTable.Button:SetVoid1(iOtherPlayer);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0465}}<syntaxhighlight lang="lua">controlTable.MinorButton:SetVoid1( iPlayerLoop );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0921}}<syntaxhighlight lang="lua">instanceControls.Button:SetVoid1( iLeaderId ); -- leader ID</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0508}}<syntaxhighlight lang="lua">Controls.SortResearch:SetVoid1( eResearch );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0510}}<syntaxhighlight lang="lua">Controls.SortCulture:SetVoid1( eCulture );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1052}}<syntaxhighlight lang="lua">Controls.ScrollBottom:SetVoid1( BOTTOM );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0366}}<syntaxhighlight lang="lua">controlTable.JoinButton:SetVoid1( serverEntry.serverID ); -- Server ID</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0159}}<syntaxhighlight lang="lua">instance.Button:SetVoid1( unit:GetID() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0358}}<syntaxhighlight lang="lua">Controls.SortMovement:SetVoid1( eMovement );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationLogPopup.lua}}
:<code>UI/InGame/Popups/NotificationLogPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0059}}<syntaxhighlight lang="lua">controlTable.Button:SetVoid1( id ); -- indicates type</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.lua}}
:<code>UI/InGame/WorldView/NotificationPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0278}}<syntaxhighlight lang="lua">button:SetVoid1( Id );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0385}}<syntaxhighlight lang="lua">Controls.GameButton:SetVoid1(  1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0387}}<syntaxhighlight lang="lua">Controls.VideoButton:SetVoid1( 3 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0451}}<syntaxhighlight lang="lua">Controls.MusicVolumeSlider:SetVoid1(   iMusicVolumeKnobID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1015}}<syntaxhighlight lang="lua">controlTable.Button:SetVoid1( orderType ); -- indicates type</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0547}}<syntaxhighlight lang="lua">Controls.ProduceResearchButton:SetVoid1( g_MAINTAIN_TECH );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1148}}<syntaxhighlight lang="lua">controlTable.Button:SetVoid1( ePurchaseEnum );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceList.lua}}
:<code>UI/InGame/ResourceList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0275}}<syntaxhighlight lang="lua">Controls.SortTradeInfo:SetVoid1( eTradeInfo );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0887}}<syntaxhighlight lang="lua">controlTable.PolicyIcon:SetVoid1( i ); -- indicates which policy</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1274}}<syntaxhighlight lang="lua">instance.EnableCheck:SetVoid1( i );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0583}}<syntaxhighlight lang="lua">thisTechButton.TechButton:SetVoid1( techID ); -- indicates tech to add to queue</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0713}}<syntaxhighlight lang="lua">thisTechButton.TechButton:SetVoid1( -1 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0554}}<syntaxhighlight lang="lua">Controls.ProposeButton:SetVoid1( PROPOSE_TYPE );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0745}}<syntaxhighlight lang="lua">Controls.UsPocketOtherPlayer:SetVoid1( 1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1909}}<syntaxhighlight lang="lua">Controls.UsTableGold:SetVoid1( 1 );</syntaxhighlight>
{{CodeLine5|1910}}<syntaxhighlight lang="lua">Controls.ThemTableGold:SetVoid1( 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1955}}<syntaxhighlight lang="lua">Controls.UsGoldAmount:SetVoid1( 1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1957}}<syntaxhighlight lang="lua">Controls.ThemGoldAmount:SetVoid1( 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1994}}<syntaxhighlight lang="lua">Controls.UsPocketGoldPerTurn:SetVoid1( 1 );</syntaxhighlight>
{{CodeLine5|1995}}<syntaxhighlight lang="lua">Controls.ThemPocketGoldPerTurn:SetVoid1( 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2124}}<syntaxhighlight lang="lua">Controls.UsPocketDefensivePact:SetVoid1( 1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2196}}<syntaxhighlight lang="lua">Controls.UsPocketTradeAgreement:SetVoid1( 1 );</syntaxhighlight>
{{CodeLine5|2197}}<syntaxhighlight lang="lua">Controls.ThemPocketTradeAgreement:SetVoid1( 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2503}}<syntaxhighlight lang="lua">Controls.ThemPocketCities:SetVoid1( 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UITestMenu.lua}}
:<code>UI/FrontEnd/UITestMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0091}}<syntaxhighlight lang="lua">Controls.SmallSlider:SetVoid1( 2 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetVoid1]]