{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Steam}}.<br/>
This is a static method, invoke it with a dot.
}}


Opens the built-in web browser of the overlay and navigates to the specified URL


=Usage=
<code>'''void''' Steam.ActivateGameOverlayToWebPage<b>(</b>'''string''' url<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|url:
|valign="top"| ''The url to navigate to.
Restrictions
:Must be a fully qualified URL (in other words, include http://)
:Only supports "http" or "file" protocols
:file protocol will only navigate to a file located in <My Documents>/My Games/Sid Meier's Civilization 5/''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
-- Navigate to the Civ 5 wiki
Steam.ActivateGameOverlayToWebPage("http://wiki.2kgames.com/civ5");</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|MainMenu.lua}}
:<code>UI/FrontEnd/MainMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0215}}<syntaxhighlight lang="lua">Steam.ActivateGameOverlayToWebPage(v.customurl);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ModsBrowser.lua}}
:<code>UI/FrontEnd/Modding/ModsBrowser.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0039}}<syntaxhighlight lang="lua">Steam.ActivateGameOverlayToWebPage("http://steamcommunity.com/workshop/browse?appid=8930");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OtherMenu.lua}}
:<code>UI/FrontEnd/OtherMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0031}}<syntaxhighlight lang="lua">Steam.ActivateGameOverlayToWebPage("http://store.steampowered.com/news/?appids=8930");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ActivateGameOverlayToWebPage]]