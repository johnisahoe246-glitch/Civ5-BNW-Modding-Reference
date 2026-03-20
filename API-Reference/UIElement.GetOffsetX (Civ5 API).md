{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' UIElement:GetOffsetX<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0721}}<syntaxhighlight lang="lua">local cityNameSize = (math.abs(Controls.NextCityButton:GetOffsetX()) * 2) - (Controls.PrevCityButton:GetSizeX());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">local textBoxSize = Controls.NameBox:GetSizeX() - Controls.LeaderName:GetOffsetX();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0229}}<syntaxhighlight lang="lua">local textBoxSize = Controls.NameBox:GetSizeX() - Controls.CivName:GetOffsetX() - 120;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0260}}<syntaxhighlight lang="lua">local textBoxSize = controlTable.NameBox:GetSizeX() - controlTable.LeaderName:GetOffsetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0067}}<syntaxhighlight lang="lua">local textBoxSize = controlTable.Button:GetSizeX() - controlTable.ButtonText:GetOffsetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0126}}<syntaxhighlight lang="lua">local textSize = controlTable.Root:GetSizeX() - controlTable.Name:GetOffsetX() - controlTable.CivIconBG:GetSizeX() + (controlTable.IconBox:GetOffsetX() /2);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0325}}<syntaxhighlight lang="lua">xAbsoluteOffset = xAbsoluteOffset + Controls.GraphsPanel:GetOffsetX() + Controls.GraphDisplay:GetOffsetX();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0386}}<syntaxhighlight lang="lua">slotInstance.PlayerNameLabel:GetOffsetX(), playerName);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0404}}<syntaxhighlight lang="lua">slotInstance.PlayerNameLabel:GetOffsetX(), Locale.ConvertTextKey("TXT_KEY_AI_NICKNAME"));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0560}}<syntaxhighlight lang="lua">Controls.PlayerNameLabel:GetOffsetX(), playerName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0985}}<syntaxhighlight lang="lua">TruncateString(Controls.ThemName, Controls.ThemTablePanel:GetSizeX() - Controls.ThemTablePanel:GetOffsetX(),</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2784}}<syntaxhighlight lang="lua">TruncateString(controlTable.Name, controlTable.ButtonSize:GetSizeX() - controlTable.Name:GetOffsetX(), szName);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetOffsetX]]