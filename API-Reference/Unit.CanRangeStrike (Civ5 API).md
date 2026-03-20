{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:CanRangeStrike<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0030}}<syntaxhighlight lang="lua">elseif pHeadSelectedUnit and pHeadSelectedUnit:CanRangeStrike() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">if pHeadSelectedUnit and pHeadSelectedUnit:CanRangeStrike() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0183}}<syntaxhighlight lang="lua">elseif unit and unit:CanRangeStrike() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0228}}<syntaxhighlight lang="lua">if (pHeadSelectedCity and pHeadSelectedCity:CanRangeStrike()) or (pHeadSelectedUnit and pHeadSelectedUnit:CanRangeStrike()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0246}}<syntaxhighlight lang="lua">if (pHeadSelectedUnit and pHeadSelectedUnit:CanRangeStrike()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanRangeStrike]]
[[Category:Civ5 Combat API|CanRangeStrike]]