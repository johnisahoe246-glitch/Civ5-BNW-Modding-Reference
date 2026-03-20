{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' UIElement:IsHidden<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Too many occurences. Only 50 out of 200 are listed.''

{{PseudoH4|AdvisorCounselPopup.lua}}
:<code>UI/InGame/Popups/AdvisorCounselPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0199}}<syntaxhighlight lang="lua">if( ContextPtr:IsHidden() == false ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Advisors.lua}}
:<code>UI/InGame/WorldView/Advisors.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0048}}<syntaxhighlight lang="lua">return (not Controls.AdvisorDisplayFront:IsHidden());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseFaithGreatPerson.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseFaithGreatPerson.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0156}}<syntaxhighlight lang="lua">ContextPtr:IsHidden() == true ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0184}}<syntaxhighlight lang="lua">if (not ContextPtr:IsHidden()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0065}}<syntaxhighlight lang="lua">if(Controls.ChooseConfirm:IsHidden())then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0250}}<syntaxhighlight lang="lua">if(not Controls.BeliefPanel:IsHidden() and g_BeliefToggleContext == contextName or contextName == nil) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0042}}<syntaxhighlight lang="lua">if (ContextPtr:IsHidden()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0816}}<syntaxhighlight lang="lua">if(Controls.WarConfirm:IsHidden())then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0061}}<syntaxhighlight lang="lua">if (Controls.WarConfirm:IsHidden() and Controls.BullyConfirm:IsHidden()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0078}}<syntaxhighlight lang="lua">if (not Controls.SellBuildingConfirm:IsHidden()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0101}}<syntaxhighlight lang="lua">if(Controls.SellBuildingConfirm:IsHidden())then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6413}}<syntaxhighlight lang="lua">if(not Controls.SearchFoundNothing:IsHidden()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0016}}<syntaxhighlight lang="lua">local m_bChatOpen = not Controls.ChatPanel:IsHidden();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0259}}<syntaxhighlight lang="lua">Controls.DiploList:SetHide( not Controls.DiploList:IsHidden() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0421}}<syntaxhighlight lang="lua">local bIsHidden = Controls.DiploList:IsHidden() == true;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0432}}<syntaxhighlight lang="lua">if ( bWantHidden ~= Controls.DiploList:IsHidden()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0416}}<syntaxhighlight lang="lua">if(ContextPtr:IsHidden() == false) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0051}}<syntaxhighlight lang="lua">if( Controls.WarConfirm:IsHidden() == false ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0595}}<syntaxhighlight lang="lua">if( Controls.MajorStack:IsHidden() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0599}}<syntaxhighlight lang="lua">if(Controls.DenounceConfirm:IsHidden() and Controls.WarConfirm:IsHidden()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0610}}<syntaxhighlight lang="lua">elseif (not Controls.WarConfirm:IsHidden()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0376}}<syntaxhighlight lang="lua">local bWasHidden = Controls.CityStack:IsHidden();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0392}}<syntaxhighlight lang="lua">local bWasHidden = Controls.TradeStack:IsHidden();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0123}}<syntaxhighlight lang="lua">Controls.MainContainer:SetHide(Controls.ModsPanel:IsHidden());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0473}}<syntaxhighlight lang="lua">if(Controls.ExitConfirm:IsHidden())then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericPopup.lua}}
:<code>UI/InGame/Popups/GenericPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0139}}<syntaxhighlight lang="lua">if uiMsg == KeyEvents.KeyDown and not ContextPtr:IsHidden() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GPList.lua}}
:<code>UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0269}}<syntaxhighlight lang="lua">local bWasHidden = Controls.EngineerStack:IsHidden();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0286}}<syntaxhighlight lang="lua">local bWasHidden = Controls.MerchantStack:IsHidden();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0303}}<syntaxhighlight lang="lua">local bWasHidden = Controls.ScientistStack:IsHidden();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0034}}<syntaxhighlight lang="lua">local bWasHidden = Controls.CityBuildingStack:IsHidden();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">local bWasHidden = Controls.ResourcesAvailableStack:IsHidden();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">local bWasHidden = Controls.ResourcesImportedStack:IsHidden();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">local bWasHidden = Controls.LocalCityStack:IsHidden();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0074}}<syntaxhighlight lang="lua">Controls.NetworkDebug:SetHide( not Controls.NetworkDebug:IsHidden() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0883}}<syntaxhighlight lang="lua">if(not Controls.DetailsResults:IsHidden()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0058}}<syntaxhighlight lang="lua">Controls.OptionsPanel:SetHide( not Controls.OptionsPanel:IsHidden() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0440}}<syntaxhighlight lang="lua">if (not Controls.OptionsPanel:IsHidden()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0355}}<syntaxhighlight lang="lua">if( Controls.GraphicsChangedPopup:IsHidden() and</syntaxhighlight>
{{CodeLine5|0356}}<syntaxhighlight lang="lua">Controls.Countdown:IsHidden() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0373}}<syntaxhighlight lang="lua">if(not graphsPanel:IsHidden()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceList.lua}}
:<code>UI/InGame/ResourceList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0170}}<syntaxhighlight lang="lua">local bWasHidden = Controls.LuxuryStack:IsHidden();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0187}}<syntaxhighlight lang="lua">local bWasHidden = Controls.StrategicStack:IsHidden();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0203}}<syntaxhighlight lang="lua">local bWasHidden = Controls.BonusStack:IsHidden();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0733}}<syntaxhighlight lang="lua">if( ContextPtr:IsHidden() == false and not PreGame.IsHotSeatGame()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0745}}<syntaxhighlight lang="lua">if (slotInstance ~= nil and not slotInstance.Root:IsHidden()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPanel.lua}}
:<code>UI/InGame/TechPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0017}}<syntaxhighlight lang="lua">if( Controls.TechPopup:IsHidden() == true ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0080}}<syntaxhighlight lang="lua">if( ContextPtr:IsHidden() == true ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1380}}<syntaxhighlight lang="lua">if( Controls.UsPocketLuxuryStack:IsHidden() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1447}}<syntaxhighlight lang="lua">if( Controls.ThemPocketLuxuryStack:IsHidden() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0684}}<syntaxhighlight lang="lua">if( self.m_Instance.HealthBar:IsHidden() == false ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsHidden]]