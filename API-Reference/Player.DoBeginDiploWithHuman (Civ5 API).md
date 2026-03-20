{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Player:DoBeginDiploWithHuman<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1082}}<syntaxhighlight lang="lua">player:DoBeginDiploWithHuman();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploGlobalRelationships.lua}}
:<code>UI/InGame/Popups/DiploGlobalRelationships.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0331}}<syntaxhighlight lang="lua">Players[ ePlayer ]:DoBeginDiploWithHuman();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0139}}<syntaxhighlight lang="lua">Players[ePlayer]:DoBeginDiploWithHuman();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DoBeginDiploWithHuman]]
[[Category:Civ5 Players API|DoBeginDiploWithHuman]]
[[Category:Civ5 Diplomacy API|DoBeginDiploWithHuman]]