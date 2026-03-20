{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ButtonBase''', {{Type5|EditBox}}, {{Type5|Grid}} and {{Type5|GridButton}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetVoid2<b>(</b>{{Type5|ProcessType}} process<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|process:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0599}}<syntaxhighlight lang="lua">controlTable.BannerButton:SetVoid2( gridPosY );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0609}}<syntaxhighlight lang="lua">controlTable.EjectGarrison:SetVoid2(cityID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0612}}<syntaxhighlight lang="lua">controlTable.CityRangeStrikeButton:SetVoid2(cityID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0618}}<syntaxhighlight lang="lua">svStrikeButton.CityRangeStrikeButton:SetVoid2(cityID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0703}}<syntaxhighlight lang="lua">controlTable.EjectGarrison:SetVoid2(instance.cityID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0706}}<syntaxhighlight lang="lua">controlTable.CityRangeStrikeButton:SetVoid2(instance.cityID);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0722}}<syntaxhighlight lang="lua">svStrikeButton.CityRangeStrikeButton:SetVoid2(instance.cityID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0466}}<syntaxhighlight lang="lua">controlTable.MinorButton:SetVoid2(  pOtherPlayer:GetCapitalCity() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.lua}}
:<code>UI/InGame/Popups/DiploRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0086}}<syntaxhighlight lang="lua">controlTable.LeaderButton:SetVoid2( city );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0367}}<syntaxhighlight lang="lua">controlTable.JoinButton:SetVoid2( 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationLogPopup.lua}}
:<code>UI/InGame/Popups/NotificationLogPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0060}}<syntaxhighlight lang="lua">controlTable.Button:SetVoid2( void );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0454}}<syntaxhighlight lang="lua">Controls.ProduceGoldButton:SetVoid2( processID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0460}}<syntaxhighlight lang="lua">Controls.ProduceResearchButton:SetVoid2( processID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1016}}<syntaxhighlight lang="lua">controlTable.Button:SetVoid2( id );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0121}}<syntaxhighlight lang="lua">controlTable.Button:SetVoid2( scenarioCivID );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0130}}<syntaxhighlight lang="lua">thisTechButtonInstance.TechButton:SetVoid2( iDiscover );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0181}}<syntaxhighlight lang="lua">thisTechButtonInstance.TechButton:SetVoid2(buttonVoid2Value);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0448}}<syntaxhighlight lang="lua">thisTechButtonInstance.TechButton:SetVoid2( 0 ); -- how many free techs</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0584}}<syntaxhighlight lang="lua">thisTechButton.TechButton:SetVoid2( numFreeTechs ); -- how many free techs</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0609}}<syntaxhighlight lang="lua">thisTechButton.TechButton:SetVoid2( 0 ); -- num free techs</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2284}}<syntaxhighlight lang="lua">controlTable.AmountEdit:SetVoid2( row.ID );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2410}}<syntaxhighlight lang="lua">Controls.UsPocketCitiesClose:SetVoid2( 1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2412}}<syntaxhighlight lang="lua">Controls.ThemPocketCitiesClose:SetVoid2( 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2676}}<syntaxhighlight lang="lua">Controls.UsPocketLeaderClose:SetVoid2( 1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2678}}<syntaxhighlight lang="lua">Controls.ThemPocketLeaderClose:SetVoid2( 0 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetVoid2]]