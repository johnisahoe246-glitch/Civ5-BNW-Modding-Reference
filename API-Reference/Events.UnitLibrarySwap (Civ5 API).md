{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.UnitLibrarySwap<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.UnitLibrarySwap.Add(''<function handler>'')</code> or invoke it directly through <code>Events.UnitLibrarySwap(''<arguments list>'')</code>.



=Source code samples=
{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0389}}<syntaxhighlight lang="lua">Events.UnitLibrarySwap( );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitLibrarySwap]]
[[Category:Civ5 Units API|UnitLibrarySwap]]