{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' PreGame.TestPassword<b>(</b>{{Type5|PlayerID}} player, '''string''' arg1<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ChangePassword.lua}}
:<code>UI/InGame/ChangePassword.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">if (PreGame.TestPassword( ePlayer, Controls.OldPasswordEditBox:GetText() ) ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0088}}<syntaxhighlight lang="lua">PreGame.TestPassword( Game.GetActivePlayer(), Controls.OldPasswordEditBox:GetText() ) ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlayerChange.lua}}
:<code>UI/InGame/PlayerChange.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0009}}<syntaxhighlight lang="lua">if (PreGame.TestPassword( Game.GetActivePlayer(), Controls.EnterPasswordEditBox:GetText() )) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">local bValid = PreGame.TestPassword( Game.GetActivePlayer(), Controls.EnterPasswordEditBox:GetText() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0075}}<syntaxhighlight lang="lua">local bValid = PreGame.TestPassword( Game.GetActivePlayer(), Controls.EnterPasswordEditBox:GetText());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|TestPassword]]
[[Category:Civ5 Game Settings API|TestPassword]]