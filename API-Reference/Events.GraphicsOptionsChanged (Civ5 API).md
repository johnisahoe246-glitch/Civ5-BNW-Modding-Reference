{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.GraphicsOptionsChanged<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.GraphicsOptionsChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.GraphicsOptionsChanged(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0751}}<syntaxhighlight lang="lua">Events.GraphicsOptionsChanged.Add(UpdateGraphicsOptionsDisplay);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GraphicsOptionsChanged]]
[[Category:Civ5 Game Settings API|GraphicsOptionsChanged]]