{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GameEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


Called before most items in the game are initialized. Was once used in scenario scripts, a different strategy was used; unclear how easy it would be to get a listener registered before it fires. Apparently does not pass any parameters.


=Usage=
<code>'''void''' GameEvents.PreGameStart<b>(</b><b>)</b></code>


'''Event Type'''
:Override: the first subscriber to return true will prevent the standard game mechanic to take place. Use it to replace the corresponding game mechanic with your own function.
::You can subscribe to this event through <code>GameEvents.PreGameStart.Add(''<function handler>'')</code>.



{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PreGameStart]]