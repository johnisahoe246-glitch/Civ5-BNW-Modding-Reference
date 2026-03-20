{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventGameMessagePopup<b>(</b>{{Type5|PopupInfo}} popupInfo<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventGameMessagePopup.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventGameMessagePopup(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|popupInfo:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvisorCounselPopup.lua}}
:<code>UI/InGame/Popups/AdvisorCounselPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0208}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup.Add( OnPopup );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Advisors.lua}}
:<code>UI/InGame/WorldView/Advisors.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup(popupInfo);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0048}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup.Add( OnPopupMessage );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityList.lua}}
:<code>UI/InGame/CityList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0034}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_ECONOMIC_OVERVIEW } );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0035}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup.Add( OnEventReceived );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|2175}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup( popupInfo );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup{</syntaxhighlight>
{{CodeLine5|0028}}<syntaxhighlight lang="lua">Type = popupType,</syntaxhighlight>
{{CodeLine5|0029}}<syntaxhighlight lang="lua">Data1 = data1,</syntaxhighlight>
{{CodeLine5|0030}}<syntaxhighlight lang="lua">Data2 = data2</syntaxhighlight>
{{CodeLine5|0031}}<syntaxhighlight lang="lua">};</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0251}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_CHOOSEPOLICY } );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0024}}<syntaxhighlight lang="lua">g_MultiPullInfo[0] = { text="TXT_KEY_ADVISOR_SCREEN_TECH_TREE_DISPLAY",        call=function() Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_TECH_TREE } ); end };</syntaxhighlight>
{{CodeLine5|0025}}<syntaxhighlight lang="lua">g_MultiPullInfo[1] = { text="TXT_KEY_DIPLOMACY_OVERVIEW",        call=function() Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_DIPLOMATIC_OVERVIEW } ); end };</syntaxhighlight>
{{CodeLine5|0026}}<syntaxhighlight lang="lua">g_MultiPullInfo[2] = { text="TXT_KEY_MILITARY_OVERVIEW",         call=function() Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_MILITARY_OVERVIEW } ); end };</syntaxhighlight>
{{CodeLine5|0027}}<syntaxhighlight lang="lua">g_MultiPullInfo[3] = { text="TXT_KEY_ECONOMIC_OVERVIEW",         call=function() Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_ECONOMIC_OVERVIEW } ); end };</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0029}}<syntaxhighlight lang="lua">g_MultiPullInfo[4] = { text="TXT_KEY_DEMOGRAPHICS",              call=function() Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_DEMOGRAPHICS} ); end };</syntaxhighlight>
{{CodeLine5|0030}}<syntaxhighlight lang="lua">g_MultiPullInfo[5] = { text="TXT_KEY_POP_NOTIFICATION_LOG",      call=function() Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_NOTIFICATION_LOG, Data1 = Game.GetActivePlayer() } ); end };</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0106}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup{</syntaxhighlight>
{{CodeLine5|0107}}<syntaxhighlight lang="lua">Type = ButtonPopupTypes.BUTTONPOPUP_ESPIONAGE_OVERVIEW,</syntaxhighlight>
{{CodeLine5|0108}}<syntaxhighlight lang="lua">};</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploList.lua}}
:<code>UI/InGame/DiploList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_DIPLOMATIC_OVERVIEW } );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0124}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_MINOR_CIVS_LIST, } );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0576}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_CITY_STATE_DIPLO, Data1 = PlayerID; } );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericPopup.lua}}
:<code>UI/InGame/Popups/GenericPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup.Add( OnDisplay );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ReligionOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ReligionOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0808}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup{</syntaxhighlight>
{{CodeLine5|0809}}<syntaxhighlight lang="lua">Type = ButtonPopupTypes.BUTTONPOPUP_RELIGION_OVERVIEW,</syntaxhighlight>
{{CodeLine5|0810}}<syntaxhighlight lang="lua">};</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPanel.lua}}
:<code>UI/InGame/TechPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0018}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_CHOOSETECH,</syntaxhighlight>
{{CodeLine5|0019}}<syntaxhighlight lang="lua">Data1 = Game.GetActivePlayer(),</syntaxhighlight>
{{CodeLine5|0020}}<syntaxhighlight lang="lua">Data3 = -1 -- this is to tell it that a tech was not just finished</syntaxhighlight>
{{CodeLine5|0021}}<syntaxhighlight lang="lua">} );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0036}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_TECH_TREE } );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0037}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_TECH_TREE, Data2 = stealingTechTargetPlayerID } );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0304}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_TECH_TREE, Data2 = -1} );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0313}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_RELIGION_OVERVIEW } );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0652}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup.Add(ActivatedPopup);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitList.lua}}
:<code>UI/InGame/UnitList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0066}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopup( { Type = ButtonPopupTypes.BUTTONPOPUP_MILITARY_OVERVIEW } );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventGameMessagePopup]]