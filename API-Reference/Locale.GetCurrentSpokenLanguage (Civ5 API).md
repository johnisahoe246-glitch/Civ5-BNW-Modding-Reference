{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|ModInfo}} Locale.GetCurrentSpokenLanguage<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0684}}<syntaxhighlight lang="lua">Controls.SpokenLanguagePull:GetButton():SetText(Locale.GetCurrentSpokenLanguage().DisplayName); --TODO: make this work like its friends -KS</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCurrentSpokenLanguage]]