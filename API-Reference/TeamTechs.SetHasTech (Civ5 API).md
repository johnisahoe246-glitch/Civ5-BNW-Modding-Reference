{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|TeamTechs}}.<br/>
This is an instance method, invoke it with a colon.
}}

Gives or removes a technology from a team. Can also work on disabled techs.


=Usage=
<code>'''void''' TeamTechs:SetHasTech<b>(</b>{{Type5|TechType}} tech, '''bool''' giveTech<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tech:
|valign="top"| ''The technology to give or remove.''
|-
|valign="top" style="padding-right:6px;"|giveTech:
|valign="top"| ''If true, gives the team this technology. If false, removes the technology.''
|}


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetHasTech]]
[[Category:Civ5 Science API|SetHasTech]]