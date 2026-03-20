{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsMinorCivUnitSpawningDisabled<b>(</b>{{Type5|PlayerID}} activePlayer<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|activePlayer:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0452}}<syntaxhighlight lang="lua">if (pPlayer:IsMinorCivUnitSpawningDisabled(iActivePlayer)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0587}}<syntaxhighlight lang="lua">local bSpawningDisabled = pPlayer:IsMinorCivUnitSpawningDisabled(iActivePlayer);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsMinorCivUnitSpawningDisabled]]
[[Category:Civ5 Units API|IsMinorCivUnitSpawningDisabled]]
[[Category:Civ5 City States API|IsMinorCivUnitSpawningDisabled]]