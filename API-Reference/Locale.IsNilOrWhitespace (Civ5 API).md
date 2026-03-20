{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''bool''' Locale.IsNilOrWhitespace<b>(</b>'''int''' name<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|name:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0707}}<syntaxhighlight lang="lua">if(not Locale.IsNilOrWhitespace(map.Name)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0710}}<syntaxhighlight lang="lua">elseif(not Locale.IsNilOrWhitespace(mapData.Name)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0866}}<syntaxhighlight lang="lua">if(not Locale.IsNilOrWhitespace(map.Description)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameSetupScreen.lua}}
:<code>UI/FrontEnd/GameSetup/GameSetupScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0340}}<syntaxhighlight lang="lua">if(not Locale.IsNilOrWhitespace(mapInfo.Name)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0350}}<syntaxhighlight lang="lua">if(not Locale.IsNilOrWhitespace(name)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0279}}<syntaxhighlight lang="lua">if(not Locale.IsNilOrWhitespace(mapData.Name)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0285}}<syntaxhighlight lang="lua">if(not Locale.IsNilOrWhitespace(mapData.Description)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0530}}<syntaxhighlight lang="lua">if(not Locale.IsNilOrWhitespace(data.CivilizationName)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0534}}<syntaxhighlight lang="lua">if(not Locale.IsNilOrWhitespace(data.LeaderName)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsNilOrWhitespace]]