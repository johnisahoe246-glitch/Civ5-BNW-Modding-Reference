{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|GenerationalInstanceManager}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' GenerationalInstanceManager:ResetInstances<b>(</b><b>)</b></code>




=Source code samples=
{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0506}}<syntaxhighlight lang="lua">g_AgentManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0937}}<syntaxhighlight lang="lua">g_MyCityManager:ResetInstances();</syntaxhighlight>
{{CodeLine5|0938}}<syntaxhighlight lang="lua">g_MyCityButtonManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1086}}<syntaxhighlight lang="lua">g_TheirCityManager:ResetInstances();</syntaxhighlight>
{{CodeLine5|1087}}<syntaxhighlight lang="lua">g_TheirCityButtonManager:ResetInstances();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1427}}<syntaxhighlight lang="lua">g_IntrigueManager:ResetInstances();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ResetInstances]]