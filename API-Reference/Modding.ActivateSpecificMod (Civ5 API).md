{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Modding.ActivateSpecificMod<b>(</b>'''string''' tutorialModId, '''unknown''' tutorialModVersion<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|tutorialModId:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|tutorialModVersion:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|LoadTutorial.lua}}
:<code>UI/FrontEnd/LoadTutorial.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0113}}<syntaxhighlight lang="lua">Modding.ActivateSpecificMod(tutorialModId, tutorialModVersion);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ScenariosMenu.lua}}
:<code>UI/FrontEnd/ScenariosMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0032}}<syntaxhighlight lang="lua">Modding.ActivateSpecificMod(entry.ModID, entry.Version);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ActivateSpecificMod]]