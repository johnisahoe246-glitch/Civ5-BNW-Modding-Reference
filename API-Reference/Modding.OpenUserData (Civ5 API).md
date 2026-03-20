{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|Slider}} Modding.OpenUserData<b>(</b>'''string''' TutorialID, '''unknown''' latestTutorialVersion<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|TutorialID:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|latestTutorialVersion:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|LoadTutorial.lua}}
:<code>UI/FrontEnd/LoadTutorial.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0227}}<syntaxhighlight lang="lua">local modUserData = Modding.OpenUserData(TutorialID, latestTutorialVersion);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|OpenUserData]]