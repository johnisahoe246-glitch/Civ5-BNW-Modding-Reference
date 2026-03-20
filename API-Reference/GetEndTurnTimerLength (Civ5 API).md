{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>'''int''' getEndTurnTimerLength<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0438}}<syntaxhighlight lang="lua">timeLeft = math.ceil(getEndTurnTimerLength() - (getEndTurnTimerLength() * percentComplete));</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|getEndTurnTimerLength]]
[[Category:Civ5 Game Settings API|getEndTurnTimerLength]]
[[Category:Civ5 Turns API|getEndTurnTimerLength]]
[[Category:Civ5 Victory API|getEndTurnTimerLength]]