{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Locale.Length<b>(</b>'''string''' info<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|info:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">local iNameLength = Locale.Length(name);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0947}}<syntaxhighlight lang="lua">local iNewLength = Locale.Length(strInfo)-9;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">if(v.DisplayName ~= nil and Locale.Length(v.DisplayName) > 0) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SupportFunctions.lua}}
:<code>UI/SupportFunctions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0040}}<syntaxhighlight lang="lua">while (sizeAfterTruncate < truncatedSize and Locale.Length(newString) > 1) do</syntaxhighlight>
{{CodeLine5|0041}}<syntaxhighlight lang="lua">newString = Locale.Substring(newString, 1, Locale.Length(newString) - 1);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0058}}<syntaxhighlight lang="lua">local maxTechNameLength = 22 - Locale.Length(Locale.Lookup("TXT_KEY_TURNS"));</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Length]]