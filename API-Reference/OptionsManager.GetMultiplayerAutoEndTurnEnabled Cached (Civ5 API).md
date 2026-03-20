{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' OptionsManager.GetMultiplayerAutoEndTurnEnabled_Cached<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0644}}<syntaxhighlight lang="lua">Controls.MultiplayerAutoEndTurnCheckbox:SetCheck(OptionsManager.GetMultiplayerAutoEndTurnEnabled_Cached());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMultiplayerAutoEndTurnEnabled_Cached]]
[[Category:Civ5 Game Settings API|GetMultiplayerAutoEndTurnEnabled_Cached]]
[[Category:Civ5 Turns API|GetMultiplayerAutoEndTurnEnabled_Cached]]
[[Category:Civ5 Victory API|GetMultiplayerAutoEndTurnEnabled_Cached]]