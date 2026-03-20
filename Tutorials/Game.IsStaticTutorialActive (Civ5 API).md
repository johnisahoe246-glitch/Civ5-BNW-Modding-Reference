{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.IsStaticTutorialActive<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0154}}<syntaxhighlight lang="lua">local isTutorialOrMultiplayer = Game and (Game.IsGameMultiPlayer() or Game.IsStaticTutorialActive());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0098}}<syntaxhighlight lang="lua">if(Game.IsStaticTutorialActive()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0179}}<syntaxhighlight lang="lua">if (Game.GetTutorialLevel() < 0 and not Game.IsStaticTutorialActive()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsStaticTutorialActive]]