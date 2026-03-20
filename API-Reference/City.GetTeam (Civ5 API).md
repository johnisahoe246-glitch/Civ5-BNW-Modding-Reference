{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|TeamID}} City:GetTeam<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">thisTeam = pHeadSelectedCity:GetTeam();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTeam]]
[[Category:Civ5 Diplomacy API|GetTeam]]