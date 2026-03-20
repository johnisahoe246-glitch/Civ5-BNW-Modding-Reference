{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Plot}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Plot:IsTradeRoute<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|PlotHelpManager.lua}}
:<code>UI/InGame/PlotHelpManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0194}}<syntaxhighlight lang="lua">if (strImprovement ~= "" or plot:IsTradeRoute()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0208}}<syntaxhighlight lang="lua">if (plot:IsTradeRoute()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsTradeRoute]]
[[Category:Civ5 Improvements API|IsTradeRoute]]
[[Category:Civ5 Trade API|IsTradeRoute]]