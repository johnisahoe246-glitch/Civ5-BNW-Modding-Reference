{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetMilitaryMight<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|Demographics.lua}}
:<code>UI/InGame/Popups/Demographics.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0294}}<syntaxhighlight lang="lua">return math.sqrt( Players[iPlayer]:GetMilitaryMight() ) * 2000;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WhosWinningPopup.lua}}
:<code>UI/InGame/Popups/WhosWinningPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0245}}<syntaxhighlight lang="lua">return pPlayer:GetMilitaryMight();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMilitaryMight]]