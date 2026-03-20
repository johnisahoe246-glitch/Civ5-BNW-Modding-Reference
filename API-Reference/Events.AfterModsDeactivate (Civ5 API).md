{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.AfterModsDeactivate<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.AfterModsDeactivate.Add(''<function handler>'')</code> or invoke it directly through <code>Events.AfterModsDeactivate(''<arguments list>'')</code>.



=Source code samples=
{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1323}}<syntaxhighlight lang="lua">Events.AfterModsDeactivate.Add(function()</syntaxhighlight>
{{CodeLine5|1324}}<syntaxhighlight lang="lua">PerformFullSync();</syntaxhighlight>
{{CodeLine5|1325}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|IconSupport.lua}}
:<code>UI/IconSupport.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">Events.AfterModsDeactivate.Add(function()</syntaxhighlight>
{{CodeLine5|0275}}<syntaxhighlight lang="lua">g_IconAtlases = nil;</syntaxhighlight>
{{CodeLine5|0276}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SelectCivilization.lua}}
:<code>UI/FrontEnd/GameSetup/SelectCivilization.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0245}}<syntaxhighlight lang="lua">Events.AfterModsDeactivate.Add(function()</syntaxhighlight>
{{CodeLine5|0246}}<syntaxhighlight lang="lua">g_bRefreshCivs = true;</syntaxhighlight>
{{CodeLine5|0247}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1321}}<syntaxhighlight lang="lua">Events.AfterModsDeactivate.Add( OnDLCChanged );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AfterModsDeactivate]]