{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''AnimBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:RegisterAnimCallback<b>(</b>('''void''' func<b>(</b>'''unknown''' control<b>)</b>) KillPopupText<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|KillPopupText:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0916}}<syntaxhighlight lang="lua">instance.AlphaAnimOut:RegisterAnimCallback( KillPopupText );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|RegisterAnimCallback]]