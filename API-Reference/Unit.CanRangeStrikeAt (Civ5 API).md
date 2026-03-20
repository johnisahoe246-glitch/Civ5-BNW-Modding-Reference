{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:CanRangeStrikeAt<b>(</b>'''int''' x, '''int''' y, '''bool''' arg2 = nil, '''bool''' noncombatAllowed = nil<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|x:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|y:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|noncombatAllowed:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Bombardment.lua}}
:<code>UI/InGame/Bombardment.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0071}}<syntaxhighlight lang="lua">if thingThatCanActuallyFire:CanRangeStrikeAt(plotX,plotY) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0192}}<syntaxhighlight lang="lua">if attacker:CanRangeStrikeAt( hexX, hexY ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0401}}<syntaxhighlight lang="lua">if pHeadSelectedUnit and pHeadSelectedUnit:CanRangeStrikeAt(plotX, plotY, true, true) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0408}}<syntaxhighlight lang="lua">elseif pHeadSelectedUnit and pHeadSelectedUnit:CanRangeStrikeAt(plotX, plotY, false, true) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0626}}<syntaxhighlight lang="lua">if pHeadSelectedUnit:CanRangeStrikeAt(plotX, plotY, true, bNoncombatAllowed) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanRangeStrikeAt]]
[[Category:Civ5 Combat API|CanRangeStrikeAt]]