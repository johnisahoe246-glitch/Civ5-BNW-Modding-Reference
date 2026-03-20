{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UIManager}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>{{Type5|PolicyBranchType}} UIManager.SetUICursor<b>(</b>{{Type5|PolicyBranchType}} oldCursor<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|oldCursor:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1181}}<syntaxhighlight lang="lua">UIManager:SetUICursor( 1 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6265}}<syntaxhighlight lang="lua">UIManager:SetUICursor( 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0702}}<syntaxhighlight lang="lua">UIManager:SetUICursor(cursorIndex);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0704}}<syntaxhighlight lang="lua">UIManager:SetUICursor(defaultCursor);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0720}}<syntaxhighlight lang="lua">UIManager:SetUICursor(1); -- busy</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|JoiningRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/JoiningRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0120}}<syntaxhighlight lang="lua">local prevCursor = UIManager:SetUICursor( 1 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0122}}<syntaxhighlight lang="lua">UIManager:SetUICursor( prevCursor );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|LoadReplayMenu.lua}}
:<code>UI/FrontEnd/LoadReplayMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0023}}<syntaxhighlight lang="lua">UIManager:SetUICursor(1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0028}}<syntaxhighlight lang="lua">UIManager:SetUICursor(0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.lua}}
:<code>UI/FrontEnd/Multiplayer/Lobby.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0149}}<syntaxhighlight lang="lua">UIManager:SetUICursor( 1 ); -- Busy</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0167}}<syntaxhighlight lang="lua">UIManager:SetUICursor( 0 ); -- Normal</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0439}}<syntaxhighlight lang="lua">oldCursor = UIManager:SetUICursor(0); -- make sure we start with the default cursor</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0496}}<syntaxhighlight lang="lua">UIManager:SetUICursor(oldCursor); -- make sure we retrun the cursor to the previous state</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetUICursor]]