{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>table('''int''' => {{Type5|SpyInfo}}) Player:GetEspionageSpies<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0113}}<syntaxhighlight lang="lua">local spies = activePlayer:GetEspionageSpies();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiscussionDialog.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0223}}<syntaxhighlight lang="lua">local agents = pAIPlayer:GetEspionageSpies();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0333}}<syntaxhighlight lang="lua">local agents = activePlayer:GetEspionageSpies();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0514}}<syntaxhighlight lang="lua">local agents = pActivePlayer:GetEspionageSpies();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialInclude_Expansion1.lua (G&K)}}
:<code>DLC/Expansion/Tutorial/TutorialInclude_Expansion1.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">local agents = player:GetEspionageSpies();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetEspionageSpies]]
[[Category:Civ5 Espionnage API|GetEspionageSpies]]