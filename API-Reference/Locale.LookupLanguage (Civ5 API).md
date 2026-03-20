{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


Lookup a textkey using another language as the primary language


=Usage=
<code>'''string''' Locale.LookupLanguage<b>(</b>'''string''' language, '''string''' key, ...<b>)</b></code>


'''Returned Value'''
:Returns the textkey if it cannot be found in the dictionary, or a translated string.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|language:
|valign="top"| ''A valid language type.''
|-
|valign="top" style="padding-right:6px;"|key:
|valign="top"| ''A valid text key.''
|-
|valign="top" style="padding-right:6px;"|...:
|valign="top"| ''none or many arguments that are used when composing the final localized string.''
|}
'''Notes'''
:This localized string may or may not be in the language specified.  With support for fall-back language support, the localization system will attempt to search all available languages for the string.


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local mainMenu = Locale.LookupLanguage("fr_FR", "TXT_KEY_MAIN_MENU");</syntaxhighlight>


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0239}}<syntaxhighlight lang="lua">Controls.CountdownMessage:SetText( Locale.LookupLanguage(g_Languages[g_chosenLanguage].Type, "TXT_KEY_OPSCREEN_LANGUAGE_TIMER") );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0242}}<syntaxhighlight lang="lua">Locale.LookupLanguage( g_Languages[g_chosenLanguage].Type, "TXT_KEY_YES_BUTTON"),</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0247}}<syntaxhighlight lang="lua">Locale.LookupLanguage( g_Languages[g_chosenLanguage].Type, "TXT_KEY_NO_BUTTON"),</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|LookupLanguage]]