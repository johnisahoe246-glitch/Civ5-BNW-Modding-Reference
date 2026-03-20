{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.GameOptionsChanged<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.GameOptionsChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.GameOptionsChanged(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0281}}<syntaxhighlight lang="lua">Events.GameOptionsChanged.Add(OnGameOptionsChanged);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MiniMapPanel.lua}}
:<code>UI/InGame/WorldView/MiniMapPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0190}}<syntaxhighlight lang="lua">Events.GameOptionsChanged.Add(UpdateOptionsPanel);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0376}}<syntaxhighlight lang="lua">Events.GameOptionsChanged.Add( OnOptionsChanged );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0714}}<syntaxhighlight lang="lua">Events.GameOptionsChanged.Add(UpdateGameOptionsDisplay);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GameOptionsChanged]]
[[Category:Civ5 Game Settings API|GameOptionsChanged]]