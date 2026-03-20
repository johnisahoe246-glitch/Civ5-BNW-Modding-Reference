{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' UI.IsAIRequestingConcessions<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0621}}<syntaxhighlight lang="lua">if (UI.IsAIRequestingConcessions()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0672}}<syntaxhighlight lang="lua">if (UI.IsAIRequestingConcessions() and iNumItemsFromUs == 0) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsAIRequestingConcessions]]