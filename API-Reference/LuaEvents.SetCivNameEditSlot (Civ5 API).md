{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|LuaEvents}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' LuaEvents.SetCivNameEditSlot<b>(</b>{{Type5|PlayerID}} slot<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>LuaEvents.SetCivNameEditSlot.Add(''<function handler>'')</code> or invoke it directly through <code>LuaEvents.SetCivNameEditSlot(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|slot:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|SetCivNames.lua}}
:<code>UI/FrontEnd/GameSetup/SetCivNames.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0292}}<syntaxhighlight lang="lua">LuaEvents.SetCivNameEditSlot.Add(function(iSlot)</syntaxhighlight>
{{CodeLine5|0293}}<syntaxhighlight lang="lua">if(iSlot > -1 ) then</syntaxhighlight>
{{CodeLine5|0294}}<syntaxhighlight lang="lua">g_EditSlot = iSlot;</syntaxhighlight>
{{CodeLine5|0295}}<syntaxhighlight lang="lua">LoadDefaults();</syntaxhighlight>
{{CodeLine5|0296}}<syntaxhighlight lang="lua">Controls.AcceptButton:SetDisabled(true);</syntaxhighlight>
{{CodeLine5|0297}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeLine5|0298}}<syntaxhighlight lang="lua">end);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|StagingRoom.lua}}
:<code>UI/FrontEnd/Multiplayer/StagingRoom.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0047}}<syntaxhighlight lang="lua">LuaEvents.SetCivNameEditSlot(0);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0183}}<syntaxhighlight lang="lua">LuaEvents.SetCivNameEditSlot(playerID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetCivNameEditSlot]]
[[Category:Civ5 Game Settings API|SetCivNameEditSlot]]