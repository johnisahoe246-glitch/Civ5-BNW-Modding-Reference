{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Unit:IsEnemyInMovementRange<b>(</b>'''bool''' arg0, '''bool''' arg1<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1245}}<syntaxhighlight lang="lua">if (v:IsEnemyInMovementRange(false, false)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1774}}<syntaxhighlight lang="lua">if (v:IsEnemyInMovementRange(true, false)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1831}}<syntaxhighlight lang="lua">if (v:IsEnemyInMovementRange(false, true)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsEnemyInMovementRange]]
[[Category:Civ5 Movement API|IsEnemyInMovementRange]]
[[Category:Civ5 Combat API|IsEnemyInMovementRange]]
[[Category:Civ5 Diplomacy API|IsEnemyInMovementRange]]