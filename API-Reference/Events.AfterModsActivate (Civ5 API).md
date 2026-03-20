{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.AfterModsActivate<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.AfterModsActivate.Add(''<function handler>'')</code> or invoke it directly through <code>Events.AfterModsActivate(''<arguments list>'')</code>.



=Source code samples=
{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1319}}<syntaxhighlight lang="lua">Events.AfterModsActivate.Add(function()</syntaxhighlight>
{{CodeLine5|1320}}<syntaxhighlight lang="lua">PerformFullSync();</syntaxhighlight>
{{CodeLine5|1321}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|IconSupport.lua}}
:<code>UI/IconSupport.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0278}}<syntaxhighlight lang="lua">Events.AfterModsActivate.Add(function()</syntaxhighlight>
{{CodeLine5|0279}}<syntaxhighlight lang="lua">g_IconAtlases = nil;</syntaxhighlight>
{{CodeLine5|0280}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0241}}<syntaxhighlight lang="lua">Events.AfterModsActivate.Add(function()</syntaxhighlight>
{{CodeLine5|0242}}<syntaxhighlight lang="lua">g_bRefreshCivs = true;</syntaxhighlight>
{{CodeLine5|0243}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AfterModsActivate]]