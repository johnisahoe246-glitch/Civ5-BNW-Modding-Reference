{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetCultureWonderMultiplier<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0577}}<syntaxhighlight lang="lua">iAmount = Players[pCity:GetOwner()]:GetCultureWonderMultiplier();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCultureWonderMultiplier]]
[[Category:Civ5 Buildings API|GetCultureWonderMultiplier]]
[[Category:Civ5 Culture API|GetCultureWonderMultiplier]]