{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.OnModsBrowserNavigateBack<b>(</b>'''table''' args<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.OnModsBrowserNavigateBack.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.OnModsBrowserNavigateBack(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|args:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0882}}<syntaxhighlight lang="lua">LuaEvents.OnModsBrowserNavigateBack.Add(function(args)</syntaxhighlight>
{{CodeLine5|0883}}<syntaxhighlight lang="lua">if(not Controls.DetailsResults:IsHidden()) then</syntaxhighlight>
{{CodeLine5|0884}}<syntaxhighlight lang="lua">SetListingsState("results");</syntaxhighlight>
{{CodeLine5|0885}}<syntaxhighlight lang="lua">args.Cancel = true;</syntaxhighlight>
{{CodeLine5|0886}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0887}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsBrowser.lua}}
:<code>UI/FrontEnd/Modding/ModsBrowser.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0010}}<syntaxhighlight lang="lua">LuaEvents.OnModsBrowserNavigateBack(args);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|OnModsBrowserNavigateBack]]