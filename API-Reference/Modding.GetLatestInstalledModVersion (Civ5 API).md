{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''unknown''' Modding.GetLatestInstalledModVersion<b>(</b>'''string''' tutorialModId<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tutorialModId:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|LoadTutorial.lua}}
:<code>UI/FrontEnd/LoadTutorial.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">local tutorialModVersion = Modding.GetLatestInstalledModVersion(tutorialModId);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0225}}<syntaxhighlight lang="lua">local latestTutorialVersion = Modding.GetLatestInstalledModVersion(TutorialID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetLatestInstalledModVersion]]