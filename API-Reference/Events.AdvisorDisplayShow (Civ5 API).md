{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.AdvisorDisplayShow<b>(</b>{{Type5|AdvisorEventInfo}} info<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.AdvisorDisplayShow.Add(''<function handler>'')</code> or invoke it directly through <code>Events.AdvisorDisplayShow(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|info:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|Advisors.lua}}
:<code>UI/InGame/WorldView/Advisors.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0253}}<syntaxhighlight lang="lua">Events.AdvisorDisplayShow.Add(OnAdvisorDisplayShow);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0530}}<syntaxhighlight lang="lua">Events.AdvisorDisplayShow(AdvisorDisplayShowData);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AdvisorDisplayShow]]