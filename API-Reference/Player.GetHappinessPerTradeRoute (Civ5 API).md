{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetHappinessPerTradeRoute<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0307}}<syntaxhighlight lang="lua">strTradeConnection = pPlayer:GetHappinessPerTradeRoute();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|HappinessInfo.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0301}}<syntaxhighlight lang="lua">strTradeConnection = pPlayer:GetHappinessPerTradeRoute() / 100;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHappinessPerTradeRoute]]
[[Category:Civ5 Improvements API|GetHappinessPerTradeRoute]]
[[Category:Civ5 Happiness API|GetHappinessPerTradeRoute]]
[[Category:Civ5 Trade API|GetHappinessPerTradeRoute]]