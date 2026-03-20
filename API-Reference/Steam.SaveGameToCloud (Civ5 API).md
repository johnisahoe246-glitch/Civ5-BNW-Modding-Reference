{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Steam}}.<br/>
This is a static method, invoke it with a dot.
}}


Saves the current game to a cloud save slot.


=Usage=
<code>'''bool''' Steam.SaveGameToCloud<b>(</b>{{Type5|SpecialistType}} slot<b>)</b></code>


'''Returned Value'''
:true on success, false on failure.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|slot:
|valign="top"| ''Must be between 1 and Steam.GetMaxCloudSaves();''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local success = Steam.SaveGameToCloud(slot2);</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">Steam.SaveGameToCloud(i);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SaveGameToCloud]]