{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetSize<b>(</b>'''table''' blockSize<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|blockSize:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0825}}<syntaxhighlight lang="lua">Controls.ProdQueueBackground:SetSize(panelSize);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1094}}<syntaxhighlight lang="lua">Controls.BoxOSlackers:SetSize( frameSize );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0113}}<syntaxhighlight lang="lua">Controls.ScrollBar:SetSize( scrollBarSize );</syntaxhighlight>
{{CodeLine5|0114}}<syntaxhighlight lang="lua">Controls.LeftScrollBar:SetSize( scrollBarSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0121}}<syntaxhighlight lang="lua">Controls.ScrollPanel:SetSize( scrollPanelSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0124}}<syntaxhighlight lang="lua">Controls.LeftScrollPanel:SetSize( leftScrollPanelSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1768}}<syntaxhighlight lang="lua">innerFrame:SetSize( frameSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1771}}<syntaxhighlight lang="lua">outerFrame:SetSize( frameSize );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1683}}<syntaxhighlight lang="lua">Controls.MyRedBar:SetSize(healthBarSize);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1688}}<syntaxhighlight lang="lua">Controls.MyYellowBar:SetSize(healthBarSize);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1693}}<syntaxhighlight lang="lua">Controls.MyGreenBar:SetSize(healthBarSize);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1709}}<syntaxhighlight lang="lua">Controls.MyDeltaBar:SetSize(damageBarSize);</syntaxhighlight>
{{CodeLine5|1710}}<syntaxhighlight lang="lua">Controls.MyDeltaBarFlash:SetSize(damageBarSize);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1728}}<syntaxhighlight lang="lua">Controls.TheirRedBar:SetSize(healthBarSize);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1733}}<syntaxhighlight lang="lua">Controls.TheirYellowBar:SetSize(healthBarSize);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1738}}<syntaxhighlight lang="lua">Controls.TheirGreenBar:SetSize(healthBarSize);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1754}}<syntaxhighlight lang="lua">Controls.TheirDeltaBar:SetSize(damageBarSize);</syntaxhighlight>
{{CodeLine5|1755}}<syntaxhighlight lang="lua">Controls.TheirDeltaBarFlash:SetSize(damageBarSize);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0734}}<syntaxhighlight lang="lua">Controls.DetailValuesStack:SetSize{x = max_detail_value_width, y =  details_size.y};</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0042}}<syntaxhighlight lang="lua">Controls.Backdrop:SetSize( backdropSize );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0269}}<syntaxhighlight lang="lua">Controls.MainBox:SetSize( frameSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">Controls.BackgroundBox:SetSize( frameSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0275}}<syntaxhighlight lang="lua">Controls.FrameBox:SetSize( frameSize );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0706}}<syntaxhighlight lang="lua">pipe.ConnectorImage:SetSize(size);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0155}}<syntaxhighlight lang="lua">hConnection.TechPipeIcon:SetSize(size);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0163}}<syntaxhighlight lang="lua">vConnection.TechPipeIcon:SetSize(size);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0204}}<syntaxhighlight lang="lua">startPipe.TechPipeIcon:SetSize(connectorSize);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0271}}<syntaxhighlight lang="lua">startPipe.TechPipeIcon:SetSize(   Vector2(40, 42) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0394}}<syntaxhighlight lang="lua">thisEraBlockInstance.EraBlock:SetSize( blockSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0397}}<syntaxhighlight lang="lua">thisEraBlockInstance.FrameBottom:SetSize( blockSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0401}}<syntaxhighlight lang="lua">thisEraBlockInstance.OldBar:SetSize( blockSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0404}}<syntaxhighlight lang="lua">thisEraBlockInstance.OldBlock:SetSize( blockSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0408}}<syntaxhighlight lang="lua">thisEraBlockInstance.CurrentBlock:SetSize( blockSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0411}}<syntaxhighlight lang="lua">thisEraBlockInstance.CurrentBlock1:SetSize( blockSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0414}}<syntaxhighlight lang="lua">thisEraBlockInstance.CurrentBlock2:SetSize( blockSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0418}}<syntaxhighlight lang="lua">thisEraBlockInstance.CurrentTop:SetSize( blockSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0421}}<syntaxhighlight lang="lua">thisEraBlockInstance.CurrentTop1:SetSize( blockSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0424}}<syntaxhighlight lang="lua">thisEraBlockInstance.CurrentTop2:SetSize( blockSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0428}}<syntaxhighlight lang="lua">thisEraBlockInstance.FutureBlock:SetSize( blockSize );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">Controls.LeaderSpeechBorderFrame:SetSize( frameSize );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0216}}<syntaxhighlight lang="lua">Controls.LeaderSpeechFrame:SetSize( frameSize );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0659}}<syntaxhighlight lang="lua">Controls.RedBar:SetSize(barSize);</syntaxhighlight>
{{CodeLine5|0660}}<syntaxhighlight lang="lua">Controls.RedAnim:SetSize(barSize);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0665}}<syntaxhighlight lang="lua">Controls.YellowBar:SetSize(barSize);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0670}}<syntaxhighlight lang="lua">Controls.GreenBar:SetSize(barSize);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetSize]]