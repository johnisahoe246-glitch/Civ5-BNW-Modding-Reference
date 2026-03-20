{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GreatAdmiralThreshold<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|GPList.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/GPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0169}}<syntaxhighlight lang="lua">local fThreshold = pPlayer:GreatAdmiralThreshold();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0094}}<syntaxhighlight lang="lua">fThreshold = pPlayer:GreatAdmiralThreshold();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GreatAdmiralThreshold]]
[[Category:Civ5 Great People API|GreatAdmiralThreshold]]