{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Player:ChangeNumWorldWonders<b>(</b>'''int''' numWondersToCredit<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|numWondersToCredit:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0175}}<syntaxhighlight lang="lua">player:ChangeNumWorldWonders( iNumWondersToCredit );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ChangeNumWorldWonders]]
[[Category:Civ5 Buildings API|ChangeNumWorldWonders]]