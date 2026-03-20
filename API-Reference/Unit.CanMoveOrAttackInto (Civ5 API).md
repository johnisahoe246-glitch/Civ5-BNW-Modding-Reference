{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Unit:CanMoveOrAttackInto<b>(</b>{{Type5|Plot}} plot, '''bool''' declareWar = false, '''bool''' destination = false<b>)</b></code>


'''Returned Value'''
:This function is bugged and always returns false if called from Lua, use unit:CanMoveThrough(plot) instead.--[[User:Killmeplease|Killmeplease]] ([[User talk:Killmeplease|talk]]) 04:12, 1 November 2015 (UTC)
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|plot:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|declareWar:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|destination:
|valign="top"| ''No description available.''
|}


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanMoveOrAttackInto]]
[[Category:Civ5 Movement API|CanMoveOrAttackInto]]
[[Category:Civ5 Combat API|CanMoveOrAttackInto]]