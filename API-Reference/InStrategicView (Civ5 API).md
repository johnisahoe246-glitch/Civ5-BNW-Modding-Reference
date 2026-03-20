{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>'''bool''' InStrategicView<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">if InStrategicView() then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0173}}<syntaxhighlight lang="lua">Controls.StrategicStack:SetHide( not InStrategicView() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0233}}<syntaxhighlight lang="lua">if(info ~= nil and InStrategicView()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0155}}<syntaxhighlight lang="lua">if( InStrategicView() )</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0110}}<syntaxhighlight lang="lua">elseif ( wParam == Keys.VK_ESCAPE and InStrategicView() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0781}}<syntaxhighlight lang="lua">g_PerPlayerStrategicViewSettings[ iPrevActivePlayer + 1 ] = InStrategicView();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0785}}<syntaxhighlight lang="lua">if (g_PerPlayerStrategicViewSettings[ iActivePlayer + 1] and not InStrategicView()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0788}}<syntaxhighlight lang="lua">if (not g_PerPlayerStrategicViewSettings[ iActivePlayer + 1] and InStrategicView()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|InStrategicView]]