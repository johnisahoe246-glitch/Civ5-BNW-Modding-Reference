{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|GameStateType}} UI.GetCurrentGameState<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0602}}<syntaxhighlight lang="lua">if( UI.GetCurrentGameState() == GameStateTypes.CIV5_GS_MAINGAMEVIEW ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0924}}<syntaxhighlight lang="lua">elseif( UI.GetCurrentGameState() == GameStateTypes.CIV5_GS_MAIN_MENU ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCurrentGameState]]