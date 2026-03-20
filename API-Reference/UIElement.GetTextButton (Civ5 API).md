{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|CheckBox}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|Button}} UIElement:GetTextButton<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0217}}<syntaxhighlight lang="lua">local gameOptionTextButton = gameOption.GameOptionRoot:GetTextButton();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1057}}<syntaxhighlight lang="lua">local victoryConditionTextButton = victoryCondition.GameOptionRoot:GetTextButton();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0989}}<syntaxhighlight lang="lua">local dlcButton = dlcEntries.GameOptionRoot:GetTextButton();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTextButton]]