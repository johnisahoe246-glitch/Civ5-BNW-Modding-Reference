{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' PreGame.IsRandomMapScript<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0044}}<syntaxhighlight lang="lua">if(PreGame.IsRandomMapScript())then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0623}}<syntaxhighlight lang="lua">local bIsMapScript = PreGame.IsRandomMapScript();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0835}}<syntaxhighlight lang="lua">if( not PreGame.IsRandomMapScript() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0886}}<syntaxhighlight lang="lua">if(PreGame.IsRandomMapScript()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0209}}<syntaxhighlight lang="lua">elseif( not PreGame.IsRandomMapScript() ) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">if ( not PreGame.IsRandomMapScript() ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsRandomMapScript]]
[[Category:Civ5 Game Settings API|IsRandomMapScript]]