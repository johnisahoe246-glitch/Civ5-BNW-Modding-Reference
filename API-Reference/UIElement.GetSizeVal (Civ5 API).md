{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''', '''int''' UIElement:GetSizeVal<b>(</b><b>)</b></code>


'''Returned Values'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0016}}<syntaxhighlight lang="lua">local spWidth, spHeight = Controls.ItemScrollPanel:GetSizeVal();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">local bpWidth, bpHeight = Controls.BottomPanel:GetSizeVal();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0114}}<syntaxhighlight lang="lua">local buttonWidth, buttonHeight = itemInstance.Button:GetSizeVal();</syntaxhighlight>
{{CodeLine5|0115}}<syntaxhighlight lang="lua">local descWidth, descHeight = itemInstance.Description:GetSizeVal();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0514}}<syntaxhighlight lang="lua">local gw,gh = itemInstance.AnimGrid:GetSizeVal();</syntaxhighlight>
{{CodeLine5|0515}}<syntaxhighlight lang="lua">local dw,dh = itemInstance.Description:GetSizeVal();</syntaxhighlight>
{{CodeLine5|0516}}<syntaxhighlight lang="lua">local bw,bh = itemInstance.Button:GetSizeVal();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0342}}<syntaxhighlight lang="lua">local width, height = Controls.ConfirmContent:GetSizeVal();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0987}}<syntaxhighlight lang="lua">local width, height = entry.PotentialMeterBack:GetSizeVal();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1480}}<syntaxhighlight lang="lua">local width, height = instance.Message:GetSizeVal();</syntaxhighlight>
{{CodeLine5|1481}}<syntaxhighlight lang="lua">local baseWidth, baseHeight = instance.Base:GetSizeVal();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1710}}<syntaxhighlight lang="lua">local width, height = Controls.NotificationContent:GetSizeVal();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0374}}<syntaxhighlight lang="lua">local bw,bh = entry.Base:GetSizeVal();</syntaxhighlight>
{{CodeLine5|0375}}<syntaxhighlight lang="lua">local bdw,bdh = entry.BeliefDescription:GetSizeVal();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0273}}<syntaxhighlight lang="lua">local baseWidth, baseHeight = messageInstance.Base:GetSizeVal();</syntaxhighlight>
{{CodeLine5|0274}}<syntaxhighlight lang="lua">local msgWidth, msgHeight = messageInstance.MessageText:GetSizeVal();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0394}}<syntaxhighlight lang="lua">local graphWidth, graphHeight = Controls.GraphCanvas:GetSizeVal();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1046}}<syntaxhighlight lang="lua">local bw,bh = controlTable.Button:GetSizeVal();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1059}}<syntaxhighlight lang="lua">local bw, bh = controlTable.Button:GetSizeVal();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1061}}<syntaxhighlight lang="lua">local tw, th = controlTable.Button:GetTextControl():GetSizeVal();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0403}}<syntaxhighlight lang="lua">local name_length = Controls.UnitName:GetSizeVal();</syntaxhighlight>
{{CodeLine5|0404}}<syntaxhighlight lang="lua">local box_length = Controls.UnitNameButton:GetSizeVal();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0410}}<syntaxhighlight lang="lua">name_length = Controls.UnitName:GetSizeVal();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WonderPopup.lua}}
:<code>UI/InGame/Popups/WonderPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">m_fOriginalSizeX, m_fOriginalSizeY = Controls.WonderSplash:GetSizeVal();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetSizeVal]]