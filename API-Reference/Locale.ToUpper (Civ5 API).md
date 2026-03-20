{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Locale}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''string''' Locale.ToUpper<b>(</b>'''string''' localizedCityName<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|localizedCityName:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0147}}<syntaxhighlight lang="lua">local convertedKey = Locale.ToUpper(localizedCityName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0719}}<syntaxhighlight lang="lua">convertedKey = Locale.ToUpper(convertedKey);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0840}}<syntaxhighlight lang="lua">szItemName = Locale.ToUpper(szItemName);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0025}}<syntaxhighlight lang="lua">name = Locale.ToUpper(name);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0385}}<syntaxhighlight lang="lua">Controls.RangedAttackButtonLabel:SetText(Locale.ToUpper(Locale.ConvertTextKey("TXT_KEY_INTERFACEMODE_RANGE_ATTACK")));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">strHelpText = strHelpText .. Locale.ToUpper(Locale.ConvertTextKey( pUnitInfo.Description ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0109}}<syntaxhighlight lang="lua">strHelpText = strHelpText .. Locale.ToUpper(Locale.ConvertTextKey( pBuildingInfo.Description ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0261}}<syntaxhighlight lang="lua">strHelpText = strHelpText .. Locale.ToUpper(Locale.ConvertTextKey( pImprovementInfo.Description ));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0302}}<syntaxhighlight lang="lua">strHelpText = strHelpText .. Locale.ToUpper(Locale.ConvertTextKey( pProjectInfo.Description ));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0654}}<syntaxhighlight lang="lua">packageID = Locale.ToUpper(packageID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ResourceTooltipGenerator.lua}}
:<code>UI/InGame/ResourceTooltipGenerator.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">local strToolTip = "[COLOR_POSITIVE_TEXT]" .. strQuantity .. Locale.ToUpper(Locale.ConvertTextKey(pResourceInfo.Description)) .. "[ENDCOLOR]";</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0024}}<syntaxhighlight lang="lua">if(Locale.ToUpper(newSave) == Locale.ToUpper(v.DisplayName)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechHelpInclude.lua}}
:<code>UI/InGame/TechTree/TechHelpInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0015}}<syntaxhighlight lang="lua">strHelpText = strHelpText .. Locale.ToUpper(Locale.ConvertTextKey( pTechInfo.Description ));</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">Controls.MenuButton:SetText(Locale.ToUpper(Locale.ConvertTextKey("TXT_KEY_RETURN")));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0021}}<syntaxhighlight lang="lua">Controls.MenuButton:SetText(Locale.ToUpper(Locale.ConvertTextKey("TXT_KEY_MENU")));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">strGoldenAgeStr = string.format(Locale.ToUpper(Locale.ConvertTextKey("TXT_KEY_GOLDEN_AGE_ANNOUNCE")) .. " (%i)", pPlayer:GetGoldenAgeTurns());</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0589}}<syntaxhighlight lang="lua">Controls.ProposeButton:SetText( Locale.ToUpper(Locale.ConvertTextKey( "TXT_KEY_DIPLO_DEMAND_BUTTON" )));</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ToUpper]]