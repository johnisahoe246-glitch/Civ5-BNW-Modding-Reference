{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendGameOptions<b>(</b>table('''int''' => table('''int''' => '''string''')) options<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|options:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0116}}<syntaxhighlight lang="lua">Network.SendGameOptions(options);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendGameOptions]]
[[Category:Civ5 Game Settings API|SendGameOptions]]