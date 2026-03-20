{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.AudioDebugChangeMusic<b>(</b>'''bool''' arg0, '''bool''' arg1, '''bool''' arg2<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.AudioDebugChangeMusic.Add(''<function handler>'')</code> or invoke it directly through <code>Events.AudioDebugChangeMusic(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''Play next song.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''Toggle war state.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''Reset audio.''
|}


=Source code samples=
{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0132}}<syntaxhighlight lang="lua">Events.AudioDebugChangeMusic(true,false,false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0136}}<syntaxhighlight lang="lua">Events.AudioDebugChangeMusic(true,true,false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">Events.AudioDebugChangeMusic(false,false,true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AudioDebugChangeMusic]]