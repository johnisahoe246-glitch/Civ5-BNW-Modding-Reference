{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' OptionsManager.GetSinglePlayerQuickCombatEnabled_Cached<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0648}}<syntaxhighlight lang="lua">Controls.SPQuickCombatCheckBox:SetCheck(OptionsManager.GetSinglePlayerQuickCombatEnabled_Cached());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetSinglePlayerQuickCombatEnabled_Cached]]
[[Category:Civ5 Combat API|GetSinglePlayerQuickCombatEnabled_Cached]]
[[Category:Civ5 Players API|GetSinglePlayerQuickCombatEnabled_Cached]]
[[Category:Civ5 Game Settings API|GetSinglePlayerQuickCombatEnabled_Cached]]