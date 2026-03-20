{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.GetWorldNumCitiesUnhappinessPercent<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|HappinessInfo.lua}}
:<code>UI/InGame/Popups/HappinessInfo.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0432}}<syntaxhighlight lang="lua">local iCityCountMod = Game:GetWorldNumCitiesUnhappinessPercent();   -- World Size</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetWorldNumCitiesUnhappinessPercent]]
[[Category:Civ5 Cities API|GetWorldNumCitiesUnhappinessPercent]]
[[Category:Civ5 Happiness API|GetWorldNumCitiesUnhappinessPercent]]