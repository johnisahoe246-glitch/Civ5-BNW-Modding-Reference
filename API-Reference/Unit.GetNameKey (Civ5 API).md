{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' Unit:GetNameKey<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ConfirmGiftPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ConfirmGiftPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">local unitNameKey = pUnit:GetNameKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0161}}<syntaxhighlight lang="lua">sortEntry.name = unit:GetNameKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PlotMouseoverInclude.lua}}
:<code>UI/InGame/PlotMouseoverInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0272}}<syntaxhighlight lang="lua">strUnitText = strUnitText .. Locale.ConvertTextKey("TXT_KEY_MULTIPLAYER_UNIT_TT", pPlayer:GetNickName(), pPlayer:GetCivilizationAdjectiveKey(), unit:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0276}}<syntaxhighlight lang="lua">local desc = Locale.ConvertTextKey("TXT_KEY_PLOTROLL_UNIT_DESCRIPTION_CIV", pPlayer:GetCivilizationAdjectiveKey(), unit:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0279}}<syntaxhighlight lang="lua">strUnitText = strUnitText .. Locale.ConvertTextKey("TXT_KEY_PLOTROLL_UNIT_DESCRIPTION_CIV", pPlayer:GetCivilizationAdjectiveKey(), unit:GetNameKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReturnCivilianPopup.lua}}
:<code>UI/InGame/PopupsGeneric/ReturnCivilianPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">local strOldUnitKey = pUnit:GetNameKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetUnitName.lua}}
:<code>UI/InGame/Popups/SetUnitName.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0120}}<syntaxhighlight lang="lua">local unitName = pUnit:GetNameKey();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0170}}<syntaxhighlight lang="lua">local desc = Locale.ConvertTextKey("TXT_KEY_PLOTROLL_UNIT_DESCRIPTION_CIV",  o.m_Player:GetCivilizationAdjectiveKey(), pUnit:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0173}}<syntaxhighlight lang="lua">unitNameString = Locale.ConvertTextKey("TXT_KEY_PLOTROLL_UNIT_DESCRIPTION_CIV",  o.m_Player:GetCivilizationAdjectiveKey(), pUnit:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0195}}<syntaxhighlight lang="lua">local string = Locale.ConvertTextKey("TXT_KEY_MULTIPLAYER_UNIT_TT", o.m_Player:GetNickName(), o.m_Player:GetCivilizationAdjectiveKey(), pUnit:GetNameKey() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0217}}<syntaxhighlight lang="lua">o.m_Instance.UnitIcon:SetToolTipString(Locale.ConvertTextKey("TXT_KEY_MULTIPLAYER_UNIT_TT", o.m_Player:GetNickName(), o.m_Player:GetCivilizationAdjectiveKey(), pUnit:GetNameKey()));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1582}}<syntaxhighlight lang="lua">toolTipString = Locale.ConvertTextKey("TXT_KEY_MULTIPLAYER_UNIT_TT", pPlayer:GetNickName(), pPlayer:GetCivilizationAdjectiveKey(), pUnit:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1585}}<syntaxhighlight lang="lua">local desc = Locale.ConvertTextKey("TXT_KEY_PLOTROLL_UNIT_DESCRIPTION_CIV",  pPlayer:GetCivilizationAdjectiveKey(), pUnit:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1588}}<syntaxhighlight lang="lua">toolTipString = Locale.ConvertTextKey("TXT_KEY_PLOTROLL_UNIT_DESCRIPTION_CIV",  pPlayer:GetCivilizationAdjectiveKey(), pUnit:GetNameKey());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0195}}<syntaxhighlight lang="lua">string = Locale.ConvertTextKey("TXT_KEY_MULTIPLAYER_UNIT_TT", o.m_Player:GetNickName(), o.m_Player:GetCivilizationAdjectiveKey(), pUnit:GetNameKey() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0131}}<syntaxhighlight lang="lua">sortEntry.name = Locale.ConvertTextKey( unit:GetNameKey() );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0723}}<syntaxhighlight lang="lua">local searchString = Locale.ConvertTextKey( unit:GetNameKey() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0736}}<syntaxhighlight lang="lua">local name = unit and unit:GetNameKey() or "unit is nil";</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNameKey]]