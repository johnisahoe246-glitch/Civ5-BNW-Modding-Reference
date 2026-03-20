{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GenerationalInstanceManager}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''table''' GenerationalInstanceManager:new<b>(</b>'''string''' instanceName, '''string''' rootControlName, {{Type5|Stack}} ParentControl<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|instanceName:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|rootControlName:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ParentControl:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0008}}<syntaxhighlight lang="lua">local g_AgentManager = GenerationalInstanceManager:new( "AgentInstance", "Base", Controls.AgentStack);</syntaxhighlight>
{{CodeLine5|0009}}<syntaxhighlight lang="lua">local g_MyCityManager = GenerationalInstanceManager:new( "MyCityInstance", "Base", Controls.MyCityStack);</syntaxhighlight>
{{CodeLine5|0010}}<syntaxhighlight lang="lua">local g_MyCityButtonManager = GenerationalInstanceManager:new("MyCityButtonInstance", "Base", Controls.MyCityStack);</syntaxhighlight>
{{CodeLine5|0011}}<syntaxhighlight lang="lua">local g_TheirCityManager = GenerationalInstanceManager:new( "TheirCityInstance", "Base", Controls.TheirCityStack);</syntaxhighlight>
{{CodeLine5|0012}}<syntaxhighlight lang="lua">local g_TheirCityButtonManager = GenerationalInstanceManager:new( "TheirCityButtonInstance", "Base", Controls.TheirCityStack);</syntaxhighlight>
{{CodeLine5|0013}}<syntaxhighlight lang="lua">local g_IntrigueManager = GenerationalInstanceManager:new( "IntrigueMessageInstance", "Base", Controls.IntrigueMessageStack);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|new]]