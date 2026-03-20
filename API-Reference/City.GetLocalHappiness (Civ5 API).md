{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetLocalHappiness<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|HappinessInfo.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0331}}<syntaxhighlight lang="lua">if (pCity:GetLocalHappiness() > 0) then</syntaxhighlight>
{{CodeLine5|0332}}<syntaxhighlight lang="lua">strLocalCity = pCity:GetLocalHappiness();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetLocalHappiness]]
[[Category:Civ5 Happiness API|GetLocalHappiness]]