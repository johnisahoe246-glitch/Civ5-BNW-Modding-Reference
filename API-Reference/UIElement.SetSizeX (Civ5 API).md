{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetSizeX<b>(</b>'''int''' width<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|width:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0763}}<syntaxhighlight lang="lua">BannerInstance.CityBannerBackgroundIcon:SetSizeX(iWidth);</syntaxhighlight>
{{CodeLine5|0764}}<syntaxhighlight lang="lua">BannerInstance.CityBannerButtonGlow:SetSizeX(iWidth);</syntaxhighlight>
{{CodeLine5|0765}}<syntaxhighlight lang="lua">BannerInstance.CityBannerButtonBase:SetSizeX(iWidth);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0778}}<syntaxhighlight lang="lua">BannerInstance.BannerButton:SetSizeX(iWidth);</syntaxhighlight>
{{CodeLine5|0779}}<syntaxhighlight lang="lua">BannerInstance.CityBannerBackground:SetSizeX(iWidth);</syntaxhighlight>
{{CodeLine5|0780}}<syntaxhighlight lang="lua">BannerInstance.CityBannerBackgroundHL:SetSizeX(iWidth);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1300}}<syntaxhighlight lang="lua">Controls.ResourceDemandedBox:SetSizeX(Controls.ResourceDemandedString:GetSizeX() + 10);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0555}}<syntaxhighlight lang="lua">Controls.DetailsGrid:SetSizeX( sizeX );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">controlTable.Root:SetSizeX(260);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0113}}<syntaxhighlight lang="lua">controlTable.ClickEntry:SetSizeX(260);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">controlTable.Seperator:SetSizeX( 235 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">controlTable.Root:SetSizeX(200);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0120}}<syntaxhighlight lang="lua">controlTable.ClickEntry:SetSizeX(200);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0122}}<syntaxhighlight lang="lua">controlTable.Seperator:SetSizeX( 175 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0245}}<syntaxhighlight lang="lua">teamEntry.Root:SetSizeX( teamEntry.TeamStack:GetSizeX() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0278}}<syntaxhighlight lang="lua">teamEntry.TeamBox:SetSizeX(260);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0280}}<syntaxhighlight lang="lua">teamEntry.TeamClickEntry:SetSizeX( 260 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0282}}<syntaxhighlight lang="lua">teamEntry.TeamSeparator:SetSizeX( 235 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0284}}<syntaxhighlight lang="lua">teamEntry.TeamBox:SetSizeX(200);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0286}}<syntaxhighlight lang="lua">teamEntry.TeamClickEntry:SetSizeX(200);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0288}}<syntaxhighlight lang="lua">teamEntry.TeamSeparator:SetSizeX( 175 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0071}}<syntaxhighlight lang="lua">Controls.TechTreeScrollBar:SetSizeX( Controls.TechTreeScrollPanel:GetSize().x - 150 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetSizeX]]