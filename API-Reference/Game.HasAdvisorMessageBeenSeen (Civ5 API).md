{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Game.HasAdvisorMessageBeenSeen<b>(</b>'''string''' tutorialID<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tutorialID:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0605}}<syntaxhighlight lang="lua">if ( (gameHasAdvisorMessageBeenSeen(tutorialID) and not isPester) or uiHasAdvisorMessageBeenSeen(tutorialID)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|HasAdvisorMessageBeenSeen]]