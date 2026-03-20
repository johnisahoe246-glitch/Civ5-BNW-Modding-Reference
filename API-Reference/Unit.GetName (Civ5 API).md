{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' Unit:GetName<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0092}}<syntaxhighlight lang="lua">local name = pUnit:GetName();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0186}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_NEWWORLD_SCENARIO_FIRST_CIRCUMNAVIGATION", unit:GetName(), iGoldReceived, iVPReceived);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0188}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_NEWWORLD_SCENARIO_SECOND_CIRCUMNAVIGATION", unit:GetName(), iGoldReceived, iVPReceived);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0190}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_NEWWORLD_SCENARIO_THIRD_CIRCUMNAVIGATION", unit:GetName(), iGoldReceived, iVPReceived);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0633}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_CARAVEL", unit:GetName(), iVPReceived, (5 - iNumCaravels));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0680}}<syntaxhighlight lang="lua">popupInfo.Text = Locale.ConvertTextKey("TXT_KEY_MEDIEVAL_SCENARIO_CONQUISTADOR", unit:GetName(), iGoldReceived, iVPReceived);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0171}}<syntaxhighlight lang="lua">unitNameString = string.format("%s (%s)", pUnit:GetName(), desc);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0695}}<syntaxhighlight lang="lua">controlTable.Button:SetText( pUnit:GetName() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0715}}<syntaxhighlight lang="lua">controlTable.Button:SetText( pPlotUnit:GetName() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1057}}<syntaxhighlight lang="lua">local unitName = pPlotUnit:GetName();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1586}}<syntaxhighlight lang="lua">toolTipString = string.format("%s (%s)", pUnit:GetName(), desc);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0394}}<syntaxhighlight lang="lua">local name = unit:GetName();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetName]]