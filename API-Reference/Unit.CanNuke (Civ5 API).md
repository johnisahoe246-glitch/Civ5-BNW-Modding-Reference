{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:CanNuke<b>(</b>{{Type5|Plot}} plot<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|plot:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">if pHeadSelectedUnit and pHeadSelectedUnit:CanNuke() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0205}}<syntaxhighlight lang="lua">if unit and unit:CanNuke() then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0264}}<syntaxhighlight lang="lua">if (pHeadSelectedUnit and pHeadSelectedUnit:CanNuke()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanNuke]]
[[Category:Civ5 Combat API|CanNuke]]