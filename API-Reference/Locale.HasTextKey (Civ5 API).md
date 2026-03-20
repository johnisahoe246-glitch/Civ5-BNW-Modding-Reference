{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


Determine if a textkey can be found in the Localization System's string dictionary


=Usage=
<code>'''bool''' Locale.HasTextKey<b>(</b>'''string''' textkey<b>)</b></code>


'''Returned Value'''
:Returns true if found, false otherwise
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|textkey:
|valign="top"| ''The key to look for in the dictionary.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local bFound = Locale.HasTextKey("TXT_KEY_MAIN_MENU");</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1814}}<syntaxhighlight lang="lua">return Locale.HasTextKey(tag);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">if(Locale.HasTextKey(name)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0172}}<syntaxhighlight lang="lua">if(v.DescriptionKey and Locale.HasTextKey(v.DescriptionKey)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0312}}<syntaxhighlight lang="lua">if(Locale.HasTextKey(serverWorldSize)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|HasTextKey]]