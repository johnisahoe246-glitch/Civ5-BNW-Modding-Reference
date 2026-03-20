{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''unknown''' Modding.GetModProperty<b>(</b>'''unknown''' arg0, '''unknown''' arg1, '''string''' arg2<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CustomMod.lua}}
:<code>UI/FrontEnd/Modding/CustomMod.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0079}}<syntaxhighlight lang="lua">local customImage = Modding.GetModProperty(customMod.ModID, customMod.Version, "Custom_Background_" .. customMod.Name);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0444}}<syntaxhighlight lang="lua">local title = Modding.GetModProperty(v.ID, v.Version, "Name");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0367}}<syntaxhighlight lang="lua">local displayName = Modding.GetModProperty(v.ModID, v.Version, "Name");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ScenariosMenu.lua}}
:<code>UI/FrontEnd/ScenariosMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0101}}<syntaxhighlight lang="lua">local foregroundImage = Modding.GetModProperty(customMod.ModID, customMod.Version, "Custom_Foreground_" .. customMod.Name);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetModProperty]]