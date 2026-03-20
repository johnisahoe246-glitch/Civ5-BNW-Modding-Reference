{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:IsHurt<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0561}}<syntaxhighlight lang="lua">if (v:IsHurt() and v:CanHeal(plot) and v:MovesLeft() > 0 and v:IsSelected()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0586}}<syntaxhighlight lang="lua">if (v:IsHurt() and v:CanHeal(plot) and v:MovesLeft() > 0) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsHurt]]
[[Category:Civ5 Combat API|IsHurt]]