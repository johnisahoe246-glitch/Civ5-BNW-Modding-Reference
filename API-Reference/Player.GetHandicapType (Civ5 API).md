{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|HandicapType}} Player:GetHandicapType<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EconomicGeneralInfo.lua}}
:<code>UI/InGame/Popups/EconomicGeneralInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0179}}<syntaxhighlight lang="lua">local iHandicap = Players[Game.GetActivePlayer()]:GetHandicapType();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0286}}<syntaxhighlight lang="lua">info = GameInfo.HandicapInfos[ Players[Game.GetActivePlayer()]:GetHandicapType() ];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReplayViewer.lua}}
:<code>UI/InGame/Popups/ReplayViewer.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1286}}<syntaxhighlight lang="lua">Difficulty = GameInfo.HandicapInfos[player:GetHandicapType()].Type,</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetHandicapType]]
[[Category:Civ5 Game Settings API|GetHandicapType]]