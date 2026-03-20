{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.OnModBrowserDeleteButtonClicked<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.OnModBrowserDeleteButtonClicked.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.OnModBrowserDeleteButtonClicked(''<arguments list>'')</code>.



=Source code samples=
{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0889}}<syntaxhighlight lang="lua">LuaEvents.OnModBrowserDeleteButtonClicked.Add(function()</syntaxhighlight>
{{CodeLine5|0890}}<syntaxhighlight lang="lua">if(g_SelectedModInfo) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0892}}<syntaxhighlight lang="lua">local modId = g_SelectedModInfo.ModId;</syntaxhighlight>
{{CodeLine5|0893}}<syntaxhighlight lang="lua">local version = g_SelectedModInfo.Version;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0895}}<syntaxhighlight lang="lua">local bCanUnsubscribeMod = Modding.CanUnsubscribeMod(modId, version);</syntaxhighlight>
{{CodeLine5|0896}}<syntaxhighlight lang="lua">local bCanDeleteMod = Modding.CanDeleteMod(modId, version);</syntaxhighlight>
{{CodeLine5|0897}}<syntaxhighlight lang="lua">if(bCanUnsubscribeMod) then</syntaxhighlight>
{{CodeLine5|0898}}<syntaxhighlight lang="lua">OnUnsubscribeMod(g_SelectedModInfo);</syntaxhighlight>
{{CodeLine5|0899}}<syntaxhighlight lang="lua">elseif(bCanDeleteMod) then</syntaxhighlight>
{{CodeLine5|0900}}<syntaxhighlight lang="lua">OnDeleteMod(g_SelectedModInfo);</syntaxhighlight>
{{CodeLine5|0901}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0902}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0903}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsBrowser.lua}}
:<code>UI/FrontEnd/Modding/ModsBrowser.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0052}}<syntaxhighlight lang="lua">Controls.SmallButton1:RegisterCallback(Mouse.eLClick, function() LuaEvents.OnModBrowserDeleteButtonClicked() end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|OnModBrowserDeleteButtonClicked]]