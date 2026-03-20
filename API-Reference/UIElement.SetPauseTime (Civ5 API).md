{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''AnimBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetPauseTime<b>(</b>'''int''' delay<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|delay:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0918}}<syntaxhighlight lang="lua">instance.SlideAnim:SetPauseTime( delay );</syntaxhighlight>
{{CodeLine5|0919}}<syntaxhighlight lang="lua">instance.AlphaAnimIn:SetPauseTime( delay );</syntaxhighlight>
{{CodeLine5|0920}}<syntaxhighlight lang="lua">instance.AlphaAnimOut:SetPauseTime( delay + 0.75 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetPauseTime]]