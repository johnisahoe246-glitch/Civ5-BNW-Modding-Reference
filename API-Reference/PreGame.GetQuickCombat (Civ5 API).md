{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' PreGame.GetQuickCombat<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0108}}<syntaxhighlight lang="lua">if (m_bInGameQuickCombatState_Cached ~= PreGame.GetQuickCombat()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0297}}<syntaxhighlight lang="lua">m_bInGameQuickCombatState_Cached = PreGame.GetQuickCombat();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetQuickCombat]]
[[Category:Civ5 Combat API|GetQuickCombat]]
[[Category:Civ5 Game Settings API|GetQuickCombat]]