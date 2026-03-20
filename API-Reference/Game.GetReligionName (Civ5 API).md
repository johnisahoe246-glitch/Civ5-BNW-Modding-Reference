{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''string''' Game.GetReligionName<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|religion:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0663}}<syntaxhighlight lang="lua">SelectReligion(g_CurrentReligionID, Game.GetReligionName(g_CurrentReligionID), religionRow.IconAtlas, religionRow.PortraitIndex);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0530}}<syntaxhighlight lang="lua">sToolTipText = sToolTipText .. Locale.Lookup( "TXT_KEY_CITY_STATE_QUEST_SPREAD_RELIGION_FORMAL", Game.GetReligionName(iQuestData1) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1104}}<syntaxhighlight lang="lua">local strReligion = Locale.ConvertTextKey(Game.GetReligionName(eReligion));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1138}}<syntaxhighlight lang="lua">local strReligion = Locale.ConvertTextKey(Game.GetReligionName(iReligionID));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0112}}<syntaxhighlight lang="lua">text = Locale.Lookup("TXT_KEY_RO_STATUS_FOUNDER", Game.GetReligionName(eReligion));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0514}}<syntaxhighlight lang="lua">Name = Locale.Lookup(Game.GetReligionName(eReligion)),</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0586}}<syntaxhighlight lang="lua">Religion = Locale.Lookup(Game.GetReligionName(eReligion)),</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0393}}<syntaxhighlight lang="lua">Controls.ReligionStatusLabel:LocalizeAndSetText(Game.GetReligionName(eReligion));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0202}}<syntaxhighlight lang="lua">string = string .. " - " .. Locale.Lookup(Game.GetReligionName(eReligion));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1098}}<syntaxhighlight lang="lua">local religionName = Game.GetReligionName(unit:GetReligion());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1109}}<syntaxhighlight lang="lua">local majorityReligionName = Locale.Lookup(Game.GetReligionName(eMajorityReligion));</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetReligionName]]
[[Category:Civ5 Religion API|GetReligionName]]