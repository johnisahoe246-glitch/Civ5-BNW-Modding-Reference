{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>table('''int''' => {{Type5|MapFileInfo}}) Modding.GetMapFiles<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0689}}<syntaxhighlight lang="lua">for _, map in ipairs(Modding.GetMapFiles()) do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMapMenu.lua}}
:<code>UI/InGame/Menus/SaveMapMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0218}}<syntaxhighlight lang="lua">for i, v in ipairs(Modding.GetMapFiles()) do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectMapType.lua}}
:<code>UI/FrontEnd/GameSetup/SelectMapType.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0129}}<syntaxhighlight lang="lua">local maps = Modding.GetMapFiles();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMapFiles]]