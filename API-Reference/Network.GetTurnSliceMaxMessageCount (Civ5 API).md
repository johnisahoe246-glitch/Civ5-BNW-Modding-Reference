{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Network.GetTurnSliceMaxMessageCount<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|NetworkDebug.lua}}
:<code>UI/InGame/NetworkDebug.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0048}}<syntaxhighlight lang="lua">Controls.MaxMessages:SetText( Network.GetTurnSliceMaxMessageCount() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0065}}<syntaxhighlight lang="lua">Network.SetTurnSliceMaxMessageCount(Network.GetTurnSliceMaxMessageCount() - 1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0073}}<syntaxhighlight lang="lua">Network.SetTurnSliceMaxMessageCount(Network.GetTurnSliceMaxMessageCount() + 1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTurnSliceMaxMessageCount]]
[[Category:Civ5 Turns API|GetTurnSliceMaxMessageCount]]