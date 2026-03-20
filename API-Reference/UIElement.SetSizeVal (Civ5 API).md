{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetSizeVal<b>(</b>'''int''' baseWidth, '''int''' newHeight<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|baseWidth:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newHeight:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0022}}<syntaxhighlight lang="lua">Controls.ItemScrollPanel:SetSizeVal(spWidth, spHeight);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0033}}<syntaxhighlight lang="lua">Controls.BottomPanel:SetSizeVal(bpWidth, bpHeight);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0120}}<syntaxhighlight lang="lua">itemInstance.Button:SetSizeVal(buttonWidth, newHeight);</syntaxhighlight>
{{CodeLine5|0121}}<syntaxhighlight lang="lua">itemInstance.Box:SetSizeVal(buttonWidth + 20, newHeight);</syntaxhighlight>
{{CodeLine5|0122}}<syntaxhighlight lang="lua">itemInstance.BounceAnim:SetSizeVal(buttonWidth + 20, newHeight + 5);</syntaxhighlight>
{{CodeLine5|0123}}<syntaxhighlight lang="lua">itemInstance.BounceGrid:SetSizeVal(buttonWidth + 20, newHeight + 5);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0521}}<syntaxhighlight lang="lua">itemInstance.Button:SetSizeVal(bw, newHeight);</syntaxhighlight>
{{CodeLine5|0522}}<syntaxhighlight lang="lua">itemInstance.AnimGrid:SetSizeVal(gw, newHeight + 5);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0343}}<syntaxhighlight lang="lua">Controls.ConfirmFrame:SetSizeVal(width + 60, height + 120);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1482}}<syntaxhighlight lang="lua">instance.Base:SetSizeVal(baseWidth, height + 22);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1711}}<syntaxhighlight lang="lua">Controls.NotificationFrame:SetSizeVal(width + 60, height + 140);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0257}}<syntaxhighlight lang="lua">listing.ProgressBar:SetSizeVal(pct * 390, ph);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">Controls.Minimap:SetSizeVal( width, height );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0376}}<syntaxhighlight lang="lua">entry.Base:SetSizeVal(bw, bdh + 18);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0281}}<syntaxhighlight lang="lua">messageInstance.Base:SetSizeVal(baseWidth, newHeight);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPanel.lua}}
:<code>UI/InGame/TechPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">Controls.ActiveStyle:SetSizeVal( numButtonsAdded*56 + 76, 126 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0112}}<syntaxhighlight lang="lua">Controls.ActiveStyle:SetSizeVal( numButtonsAdded*56 + 130, 126 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1065}}<syntaxhighlight lang="lua">controlTable.Button:SetSizeVal(newWidth,bh);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0301}}<syntaxhighlight lang="lua">Controls.PrimaryStretchy:SetSizeVal( stretchySize.x, stackSize.y + buildCityButtonSize + 348 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0324}}<syntaxhighlight lang="lua">Controls.SecondaryStretchy:SetSizeVal( stretchySize.x, stackSize.y + 290 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0356}}<syntaxhighlight lang="lua">Controls.WorkerActionPanel:SetSizeVal( stackSize.x, math.floor((numBuildActions-1) / numberOfButtonsPerRow) * buttonSize + buttonPadding + buttonOffsetY + rbOffset + workerPanelSizeOffsetY );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WonderPopup.lua}}
:<code>UI/InGame/Popups/WonderPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0050}}<syntaxhighlight lang="lua">Controls.WonderSplash:SetSizeVal( m_fOriginalSizeX * (1 + m_fScaleFactor), m_fOriginalSizeY * (1 + m_fScaleFactor) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0109}}<syntaxhighlight lang="lua">Controls.WonderSplash:SetSizeVal( m_fOriginalSizeX, m_fOriginalSizeY );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0112}}<syntaxhighlight lang="lua">Controls.WonderSplash:SetSizeVal( m_fOriginalSizeX * fScale,</syntaxhighlight>
{{CodeLine5|0113}}<syntaxhighlight lang="lua">m_fOriginalSizeY * fScale );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetSizeVal]]