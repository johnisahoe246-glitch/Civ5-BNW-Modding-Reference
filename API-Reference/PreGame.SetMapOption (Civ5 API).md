{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetMapOption<b>(</b>'''unknown''' arg0, '''bool''' check<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|check:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0121}}<syntaxhighlight lang="lua">PreGame.SetMapOption(option.ID, possibleValue.Value);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0233}}<syntaxhighlight lang="lua">PreGame.SetMapOption(option.ID, bCheck);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetMapOption]]
[[Category:Civ5 Game Settings API|SetMapOption]]