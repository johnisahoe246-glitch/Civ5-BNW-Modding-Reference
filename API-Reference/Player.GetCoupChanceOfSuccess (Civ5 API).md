{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''' Player:GetCoupChanceOfSuccess<b>(</b>'''int''' city<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|city:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0722}}<syntaxhighlight lang="lua">Controls.ConfirmText:LocalizeAndSetText("TXT_KEY_EO_STAGE_COUP_QUESTION", v.Rank, v.Name, city:GetNameKey(), Players[iCityAlly]:GetCivilizationAdjectiveKey(), Players[Game.GetActivePlayer()]:GetCoupChanceOfSuccess(city), city:GetNameKey(), Players[iCityAlly]:GetCivilizationDescriptionKey(), city:GetNameKey(), v.Rank, v.Name, city:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0747}}<syntaxhighlight lang="lua">agentEntry.StageCoupButton:LocalizeAndSetToolTip("TXT_KEY_EO_SPY_COUP_ENABLED_TT", v.Rank, v.Name, city:GetNameKey(), Players[iCityAlly]:GetCivilizationAdjectiveKey(), Players[Game.GetActivePlayer()]:GetCoupChanceOfSuccess(city), v.Rank, v.Name, city:GetNameKey(), Players[iCityAlly]:GetCivilizationShortDescriptionKey(), v.Rank, v.Name, city:GetNameKey());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetCoupChanceOfSuccess]]