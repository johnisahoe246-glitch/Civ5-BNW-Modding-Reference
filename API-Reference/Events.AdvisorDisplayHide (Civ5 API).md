{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.AdvisorDisplayHide<b>(</b><b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.AdvisorDisplayHide.Add(''<function handler>'')</code> or invoke it directly through <code>Events.AdvisorDisplayHide(''<arguments list>'')</code>.



=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|Advisors.lua}}
:<code>UI/InGame/WorldView/Advisors.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0162}}<syntaxhighlight lang="lua">Events.AdvisorDisplayHide();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0259}}<syntaxhighlight lang="lua">Events.AdvisorDisplayHide.Add( OnClearAdvice );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0650}}<syntaxhighlight lang="lua">Events.AdvisorDisplayHide.Add(HandleAdvisorUIHide);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AdvisorDisplayHide]]