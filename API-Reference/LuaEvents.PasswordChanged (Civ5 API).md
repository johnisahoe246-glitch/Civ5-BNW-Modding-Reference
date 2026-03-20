{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.PasswordChanged<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.PasswordChanged.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.PasswordChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ChangePassword.lua}}
:<code>UI/InGame/ChangePassword.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">LuaEvents.PasswordChanged( Game.GetActivePlayer() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlayerChange.lua}}
:<code>UI/InGame/PlayerChange.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0147}}<syntaxhighlight lang="lua">LuaEvents.PasswordChanged.Add( function(ePlayer)</syntaxhighlight>
{{CodeLine5|0148}}<syntaxhighlight lang="lua">OnPasswordChanged( ePlayer );</syntaxhighlight>
{{CodeLine5|0149}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|PasswordChanged]]
[[Category:Civ5 Game Settings API|PasswordChanged]]