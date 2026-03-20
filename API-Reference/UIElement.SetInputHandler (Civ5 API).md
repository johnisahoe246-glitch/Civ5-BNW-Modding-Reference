{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Context}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetInputHandler<b>(</b>('''void''' func<b>(</b>{{Type5|MouseEventType}} uiMsg, {{Type5|KeyType}} wParam, '''unknown''' lParam<b>)</b>) InputHandler<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|InputHandler:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1275}}<syntaxhighlight lang="lua">ContextPtr:SetInputHandler( InputHandler );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CustomMod.lua}}
:<code>UI/FrontEnd/Modding/CustomMod.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">ContextPtr:SetInputHandler( function(uiMsg, wParam, lParam)</syntaxhighlight>
{{CodeLine5|0050}}<syntaxhighlight lang="lua">if uiMsg == KeyEvents.KeyDown then</syntaxhighlight>
{{CodeLine5|0051}}<syntaxhighlight lang="lua">if wParam == Keys.VK_ESCAPE then</syntaxhighlight>
{{CodeLine5|0052}}<syntaxhighlight lang="lua">OnBack();</syntaxhighlight>
{{CodeLine5|0053}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0054}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0055}}<syntaxhighlight lang="lua">return true;</syntaxhighlight>
{{CodeLine5|0056}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EULA.lua}}
:<code>UI/FrontEnd/Modding/EULA.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">ContextPtr:SetInputHandler(function(uiMsg, wParam, lParam)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0028}}<syntaxhighlight lang="lua">if uiMsg == KeyEvents.KeyDown then</syntaxhighlight>
{{CodeLine5|0029}}<syntaxhighlight lang="lua">if wParam == Keys.VK_ESCAPE then</syntaxhighlight>
{{CodeLine5|0030}}<syntaxhighlight lang="lua">NavigateBack();</syntaxhighlight>
{{CodeLine5|0031}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0032}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0034}}<syntaxhighlight lang="lua">return true;</syntaxhighlight>
{{CodeLine5|0035}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0034}}<syntaxhighlight lang="lua">ContextPtr:SetInputHandler( function(uiMsg, wParam, lParam)</syntaxhighlight>
{{CodeLine5|0035}}<syntaxhighlight lang="lua">if uiMsg == KeyEvents.KeyDown then</syntaxhighlight>
{{CodeLine5|0036}}<syntaxhighlight lang="lua">if wParam == Keys.VK_ESCAPE or wParam == Keys.VK_RETURN then</syntaxhighlight>
{{CodeLine5|0037}}<syntaxhighlight lang="lua">OnBack();</syntaxhighlight>
{{CodeLine5|0038}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0039}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0040}}<syntaxhighlight lang="lua">return true;</syntaxhighlight>
{{CodeLine5|0041}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsBrowser.lua}}
:<code>UI/FrontEnd/Modding/ModsBrowser.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0033}}<syntaxhighlight lang="lua">ContextPtr:SetInputHandler(InputHandler);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsMenu.lua}}
:<code>UI/FrontEnd/Modding/ModsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">ContextPtr:SetInputHandler( function(uiMsg, wParam, lParam)</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">if uiMsg == KeyEvents.KeyDown then</syntaxhighlight>
{{CodeLine5|0076}}<syntaxhighlight lang="lua">if wParam == Keys.VK_ESCAPE then</syntaxhighlight>
{{CodeLine5|0077}}<syntaxhighlight lang="lua">NavigateBack();</syntaxhighlight>
{{CodeLine5|0078}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0079}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0081}}<syntaxhighlight lang="lua">return true;</syntaxhighlight>
{{CodeLine5|0082}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotHelpManager.lua}}
:<code>UI/InGame/PlotHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0030}}<syntaxhighlight lang="lua">ContextPtr:SetInputHandler( ProcessInput );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VictoryStatus.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/VictoryStatus.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0222}}<syntaxhighlight lang="lua">ContextPtr:SetInputHandler(function(uiMsg, wParam, lParam)</syntaxhighlight>
{{CodeLine5|0223}}<syntaxhighlight lang="lua">if(uiMsg == KeyEvents.KeyDown) then</syntaxhighlight>
{{CodeLine5|0224}}<syntaxhighlight lang="lua">if (wParam == Keys.VK_ESCAPE or wParam == Keys.VK_RETURN) then</syntaxhighlight>
{{CodeLine5|0225}}<syntaxhighlight lang="lua">OnClose();</syntaxhighlight>
{{CodeLine5|0226}}<syntaxhighlight lang="lua">return true;</syntaxhighlight>
{{CodeLine5|0227}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0228}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0229}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetInputHandler]]