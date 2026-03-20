{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''unknown''' Locale.ToLower<b>(</b>'''string''' name<b>)</b></code>


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

{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0222}}<syntaxhighlight lang="lua">searchableList[Locale.ToLower(name)] = article;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6244}}<syntaxhighlight lang="lua">article = searchableList[Locale.ToLower(searchString)];</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6345}}<syntaxhighlight lang="lua">lowerCaseSearchString = Locale.ToLower(searchString);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6358}}<syntaxhighlight lang="lua">if string.find(Locale.ToLower(v.entryName), lowerCaseSearchString) ~= nil then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|6364}}<syntaxhighlight lang="lua">article = searchableList[Locale.ToLower(partialMatch[1])];</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">local mapScriptFileName = Locale.ToLower(PreGame.GetMapScript());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0056}}<syntaxhighlight lang="lua">if(Locale.ToLower(mapEntry.FileName) == mapScriptFileName) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0189}}<syntaxhighlight lang="lua">if(Locale.ToLower(map.File) == mapScriptFileName) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0231}}<syntaxhighlight lang="lua">if(string.find(Locale.ToLower(mapEntry.FileName), "continents") ~= nil) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ToLower]]