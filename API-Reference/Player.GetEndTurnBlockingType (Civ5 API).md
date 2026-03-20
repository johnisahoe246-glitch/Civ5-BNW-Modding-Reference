{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|EndTurnBlockingType}} Player:GetEndTurnBlockingType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">local blockingType = player:GetEndTurnBlockingType();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0283}}<syntaxhighlight lang="lua">local EndTurnBlockingType = player:GetEndTurnBlockingType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2584}}<syntaxhighlight lang="lua">if (pPlayer:GetEndTurnBlockingType() == EndTurnBlockingTypes.NO_ENDTURN_BLOCKING_TYPE) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetEndTurnBlockingType]]
[[Category:Civ5 Game Settings API|GetEndTurnBlockingType]]
[[Category:Civ5 Turns API|GetEndTurnBlockingType]]
[[Category:Civ5 Victory API|GetEndTurnBlockingType]]