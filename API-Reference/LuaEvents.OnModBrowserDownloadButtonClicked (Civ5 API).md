{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.OnModBrowserDownloadButtonClicked<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.OnModBrowserDownloadButtonClicked.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.OnModBrowserDownloadButtonClicked(''<arguments list>'')</code>.



=Source code samples=
{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0905}}<syntaxhighlight lang="lua">LuaEvents.OnModBrowserDownloadButtonClicked.Add(function()</syntaxhighlight>
{{CodeLine5|0906}}<syntaxhighlight lang="lua">-- Only perform actions if this panel is visible</syntaxhighlight>
{{CodeLine5|0907}}<syntaxhighlight lang="lua">if(not ContextPtr:IsHidden()) then</syntaxhighlight>
{{CodeLine5|0908}}<syntaxhighlight lang="lua">if(Modding.HasPendingInstalls()) then</syntaxhighlight>
{{CodeLine5|0909}}<syntaxhighlight lang="lua">SetListingsState("installing");</syntaxhighlight>
{{CodeLine5|0910}}<syntaxhighlight lang="lua">local status = Modding.InstallMods();</syntaxhighlight>
{{CodeLine5|0911}}<syntaxhighlight lang="lua">else</syntaxhighlight>
{{CodeLine5|0912}}<syntaxhighlight lang="lua">--Check for Updates</syntaxhighlight>
{{CodeLine5|0913}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0914}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0915}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|OnModBrowserDownloadButtonClicked]]