{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|TeamID}} Unit:GetDeclareWarRangeStrike<b>(</b>{{Type5|Plot}} plot<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|plot:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|WorldView.lua}}
:<code>UI/InGame/WorldView/WorldView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0410}}<syntaxhighlight lang="lua">local eRivalTeam = pHeadSelectedUnit:GetDeclareWarRangeStrike(plot);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetDeclareWarRangeStrike]]
[[Category:Civ5 Combat API|GetDeclareWarRangeStrike]]
[[Category:Civ5 Diplomacy API|GetDeclareWarRangeStrike]]