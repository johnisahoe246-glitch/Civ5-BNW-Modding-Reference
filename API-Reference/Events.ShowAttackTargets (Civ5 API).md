{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.ShowAttackTargets<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} arg1<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.ShowAttackTargets.Add(''<function handler>'')</code> or invoke it directly through <code>Events.ShowAttackTargets(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0619}}<syntaxhighlight lang="lua">Events.ShowAttackTargets(iPlayerID, unit:GetID());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ShowAttackTargets]]
[[Category:Civ5 Combat API|ShowAttackTargets]]