{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|Vector2}} UIElement:GetSize<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0131}}<syntaxhighlight lang="lua">local size = barMarkerCtrl:GetSize().x;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">local g_iPortraitSize = Controls.ProductionPortrait:GetSize().x;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0782}}<syntaxhighlight lang="lua">local panelSize = Controls.ProdQueueBackground:GetSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">local scrollBarWidth = Controls.ScrollBar:GetSize().x;</syntaxhighlight>
{{CodeLine5|0111}}<syntaxhighlight lang="lua">local scrollPanelSize = Controls.ScrollPanel:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0122}}<syntaxhighlight lang="lua">local leftScrollPanelSize = Controls.LeftScrollPanel:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1765}}<syntaxhighlight lang="lua">contentSize = label:GetSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua}}
:<code>UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">local contentSize = Controls.LeaderSpeech:GetSize().y + offsetOfString + bonusPadding;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0017}}<syntaxhighlight lang="lua">local g_iPortraitSize = Controls.UnitPortrait:GetSize().x;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0541}}<syntaxhighlight lang="lua">local size = detail.Label:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0550}}<syntaxhighlight lang="lua">size = detailValue.Label:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0600}}<syntaxhighlight lang="lua">local details_size = Controls.DetailsBox:GetSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0267}}<syntaxhighlight lang="lua">frameSize = Controls.MainBox:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0270}}<syntaxhighlight lang="lua">frameSize = Controls.BackgroundBox:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0273}}<syntaxhighlight lang="lua">frameSize = Controls.FrameBox:GetSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPanel.lua}}
:<code>UI/InGame/TechPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0012}}<syntaxhighlight lang="lua">local techPortraitSize = Controls.TechIcon:GetSize().x;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0071}}<syntaxhighlight lang="lua">Controls.TechTreeScrollBar:SetSizeX( Controls.TechTreeScrollPanel:GetSize().x - 150 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0392}}<syntaxhighlight lang="lua">local blockSize = thisEraBlockInstance.EraBlock:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0395}}<syntaxhighlight lang="lua">blockSize = thisEraBlockInstance.FrameBottom:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0399}}<syntaxhighlight lang="lua">blockSize = thisEraBlockInstance.OldBar:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0402}}<syntaxhighlight lang="lua">blockSize = thisEraBlockInstance.OldBlock:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0406}}<syntaxhighlight lang="lua">blockSize = thisEraBlockInstance.CurrentBlock:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0409}}<syntaxhighlight lang="lua">blockSize = thisEraBlockInstance.CurrentBlock1:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0412}}<syntaxhighlight lang="lua">blockSize = thisEraBlockInstance.CurrentBlock2:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0416}}<syntaxhighlight lang="lua">blockSize = thisEraBlockInstance.CurrentTop:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0419}}<syntaxhighlight lang="lua">blockSize = thisEraBlockInstance.CurrentTop1:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0422}}<syntaxhighlight lang="lua">blockSize = thisEraBlockInstance.CurrentTop2:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0426}}<syntaxhighlight lang="lua">blockSize = thisEraBlockInstance.FutureBlock:GetSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">local contentSize = Controls.DiscussionText:GetSize().y + offsetOfString + bonusPadding;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0024}}<syntaxhighlight lang="lua">local unitPortraitSize = Controls.UnitPortrait:GetSize().x;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0292}}<syntaxhighlight lang="lua">local stretchySize = Controls.PrimaryStretchy:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0323}}<syntaxhighlight lang="lua">stretchySize = Controls.SecondaryStretchy:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0331}}<syntaxhighlight lang="lua">stackSize = Controls.WorkerActionPanel:GetSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0292}}<syntaxhighlight lang="lua">local stackSize = Controls.PrimaryStack:GetSize();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0323}}<syntaxhighlight lang="lua">stackSize = Controls.SecondaryStack:GetSize();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetSize]]