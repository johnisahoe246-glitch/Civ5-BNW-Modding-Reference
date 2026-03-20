{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:GetReverseGreatGeneralModifier<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0780}}<syntaxhighlight lang="lua">if (pMyUnit:GetReverseGreatGeneralModifier() ~= 0) then</syntaxhighlight>
{{CodeLine5|0781}}<syntaxhighlight lang="lua">iModifier = pMyUnit:GetReverseGreatGeneralModifier();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1166}}<syntaxhighlight lang="lua">if (pTheirUnit:GetReverseGreatGeneralModifier() ~= 0) then</syntaxhighlight>
{{CodeLine5|1167}}<syntaxhighlight lang="lua">iModifier = pTheirUnit:GetReverseGreatGeneralModifier();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetReverseGreatGeneralModifier]]
[[Category:Civ5 Great People API|GetReverseGreatGeneralModifier]]
[[Category:Civ5 Combat API|GetReverseGreatGeneralModifier]]