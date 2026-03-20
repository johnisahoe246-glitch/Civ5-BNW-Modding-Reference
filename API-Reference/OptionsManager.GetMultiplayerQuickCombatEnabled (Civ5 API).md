{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''unknown''' OptionsManager.GetMultiplayerQuickCombatEnabled<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|MPGameSetupScreen.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0125}}<syntaxhighlight lang="lua">PreGame.SetQuickCombat( OptionsManager.GetMultiplayerQuickCombatEnabled() );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMultiplayerQuickCombatEnabled]]
[[Category:Civ5 Combat API|GetMultiplayerQuickCombatEnabled]]
[[Category:Civ5 Game Settings API|GetMultiplayerQuickCombatEnabled]]