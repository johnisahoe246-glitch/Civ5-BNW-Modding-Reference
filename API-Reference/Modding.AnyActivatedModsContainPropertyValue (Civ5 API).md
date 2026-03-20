{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' Modding.AnyActivatedModsContainPropertyValue<b>(</b>'''string''' arg0, '''string''' arg1<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|GameMenu.lua}}
:<code>UI/InGame/Menus/GameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0148}}<syntaxhighlight lang="lua">bDisableQuickSave = bDisableQuickSave      or Modding.AnyActivatedModsContainPropertyValue("DisableQuickSave", "1");</syntaxhighlight>
{{CodeLine5|0149}}<syntaxhighlight lang="lua">bHideLoadGameOption = bHideLoadGameOption   or Modding.AnyActivatedModsContainPropertyValue("DisableLoadGameOption", "1");</syntaxhighlight>
{{CodeLine5|0150}}<syntaxhighlight lang="lua">bHideSaveGameOption = bHideSaveGameOption   or Modding.AnyActivatedModsContainPropertyValue("DisableSaveGameOption", "1");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0618}}<syntaxhighlight lang="lua">Modding.AnyActivatedModsContainPropertyValue( "DisableSaveMapOption", "1" ) or</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AnyActivatedModsContainPropertyValue]]