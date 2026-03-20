{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GenerationalInstanceManager}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' GenerationalInstanceManager:GetInstance<b>(</b><b>)</b></code>




=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0542}}<syntaxhighlight lang="lua">local agentEntry = g_AgentManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1036}}<syntaxhighlight lang="lua">local cityEntry = g_MyCityManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1042}}<syntaxhighlight lang="lua">local cityEntry = g_MyCityButtonManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1336}}<syntaxhighlight lang="lua">local cityEntry = g_TheirCityManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1343}}<syntaxhighlight lang="lua">local cityEntry = g_TheirCityButtonManager:GetInstance();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1475}}<syntaxhighlight lang="lua">local instance = g_IntrigueManager:GetInstance();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetInstance]]