{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|OptionsManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' OptionsManager.GetSinglePlayerAutoEndTurnEnabled_Cached<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|OptionsMenu.lua}}
:<code>UI/Options/OptionsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0643}}<syntaxhighlight lang="lua">Controls.SinglePlayerAutoEndTurnCheckBox:SetCheck(OptionsManager.GetSinglePlayerAutoEndTurnEnabled_Cached());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetSinglePlayerAutoEndTurnEnabled_Cached]]
[[Category:Civ5 Players API|GetSinglePlayerAutoEndTurnEnabled_Cached]]
[[Category:Civ5 Game Settings API|GetSinglePlayerAutoEndTurnEnabled_Cached]]
[[Category:Civ5 Turns API|GetSinglePlayerAutoEndTurnEnabled_Cached]]
[[Category:Civ5 Victory API|GetSinglePlayerAutoEndTurnEnabled_Cached]]