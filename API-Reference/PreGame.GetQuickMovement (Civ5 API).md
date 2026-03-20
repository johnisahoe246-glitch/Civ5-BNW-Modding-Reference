{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' PreGame.GetQuickMovement<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0112}}<syntaxhighlight lang="lua">if (m_bInGameQuickMovementState_Cached ~= PreGame.GetQuickMovement()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0298}}<syntaxhighlight lang="lua">m_bInGameQuickMovementState_Cached = PreGame.GetQuickMovement();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetQuickMovement]]
[[Category:Civ5 Movement API|GetQuickMovement]]
[[Category:Civ5 Game Settings API|GetQuickMovement]]