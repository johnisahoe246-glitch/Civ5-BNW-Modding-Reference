{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.UnitSelectionChanged<b>(</b>{{Type5|PlayerID}} player, {{Type5|UnitID}} u, '''float''' hexX, '''float''' hexY, '''int''' k, '''bool''' isSelected, '''bool''' arg6<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.UnitSelectionChanged.Add(''<function handler>'')</code> or invoke it directly through <code>Events.UnitSelectionChanged(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|player:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|u:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|hexX:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|hexY:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|k:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|isSelected:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg6:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0216}}<syntaxhighlight lang="lua">Events.UnitSelectionChanged.Add( OnDirty );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMode.lua}}
:<code>UI/InGame/DebugMode.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0436}}<syntaxhighlight lang="lua">Events.UnitSelectionChanged(playerID, -1, 0, 0, 0, false, false);         -- Does this even work?  We want to essentially deselect the currently selected unit.  cvUnitSimSystem::OnUnitSelected does not seem to handle unitID == -1</syntaxhighlight>
{{CodeLine5|0437}}<syntaxhighlight lang="lua">Events.UnitSelectionChanged(-1, -1, iHexX, iHexY, 0, true, true);         -- cvUnitSimSystem::OnUnitSelected checks for a -1 in the PlayerID field to determine if it should use the plot location.</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0760}}<syntaxhighlight lang="lua">Events.UnitSelectionChanged.Add( OnUnitSelectionChange );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1204}}<syntaxhighlight lang="lua">Events.UnitSelectionChanged.Add( OnUnitSelect );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">Events.UnitSelectionChanged.Add( OnChangeEvent );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0750}}<syntaxhighlight lang="lua">Events.UnitSelectionChanged(playerID, g_lastUnitID, 0, 0, 0, false, false);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0754}}<syntaxhighlight lang="lua">Events.UnitSelectionChanged(playerID, unitID, hexPosition.x, hexPosition.y, 0, true, false);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|UnitSelectionChanged]]
[[Category:Civ5 Units API|UnitSelectionChanged]]