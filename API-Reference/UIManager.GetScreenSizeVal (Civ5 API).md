{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UIManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''', '''int''' UIManager.GetScreenSizeVal<b>(</b><b>)</b></code>


'''Returned Values'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1294}}<syntaxhighlight lang="lua">local _, screenY = UIManager:GetScreenSizeVal();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">local screenSizeX, screenSizeY = UIManager:GetScreenSizeVal()</syntaxhighlight>
{{CodeLine5|0016}}<syntaxhighlight lang="lua">local spWidth, spHeight = Controls.ItemScrollPanel:GetSizeVal();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">local screenSizeX, screenSizeY = UIManager:GetScreenSizeVal();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0109}}<syntaxhighlight lang="lua">local _, screenSizeY = UIManager:GetScreenSizeVal(); -- Controls.BackDrop:GetSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0030}}<syntaxhighlight lang="lua">local screenSizeX, screenSizeY = UIManager:GetScreenSizeVal()</syntaxhighlight>
{{CodeLine5|0031}}<syntaxhighlight lang="lua">local scrollPanelSize = Controls.ScrollPanel:GetSize();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0322}}<syntaxhighlight lang="lua">local screenX, screenY = UIManager:GetScreenSizeVal();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetScreenSizeVal]]