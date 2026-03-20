{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventGameMessagePopupProcessed<b>(</b>{{Type5|ButtonPopupType}} mostRecentPopup, '''int''' arg1<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventGameMessagePopupProcessed.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventGameMessagePopupProcessed(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|mostRecentPopup:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvisorCounselPopup.lua}}
:<code>UI/InGame/Popups/AdvisorCounselPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0308}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_ADVISOR_COUNSEL, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorInfoPopup.lua}}
:<code>UI/InGame/Popups/AdvisorInfoPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0295}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_ADVISOR_INFO, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|AdvisorModal.lua}}
:<code>UI/InGame/Popups/AdvisorModal.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0141}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_ADVISOR_MODAL, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|BarbarianCampPopup.lua}}
:<code>UI/InGame/Popups/BarbarianCampPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0056}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_BARBARIAN_CAMP_REWARD, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseFaithGreatPerson.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseFaithGreatPerson.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0174}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_CHOOSE_FREE_GREAT_PERSON, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0192}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(g_PopupInfo.Type, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0842}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_CITY_STATE_DIPLO, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateDiploPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0085}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(m_PopupInfo.Type, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploOverview.lua}}
:<code>UI/InGame/Popups/DiploOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0119}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_DIPLOMATIC_OVERVIEW, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0142}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_DIPLO_VOTE, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EconomicOverview.lua}}
:<code>UI/InGame/Popups/EconomicOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0072}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_ECONOMIC_OVERVIEW, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GenericPopup.lua}}
:<code>UI/InGame/Popups/GenericPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate( mostRecentPopup, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GoldenAgePopup.lua}}
:<code>UI/InGame/Popups/GoldenAgePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0056}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_GOLDEN_AGE_REWARD, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GoodyHutPopup.lua}}
:<code>UI/InGame/Popups/GoodyHutPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_GOODY_HUT_REWARD, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GreatPersonRewardPopup.lua}}
:<code>UI/InGame/Popups/GreatPersonRewardPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0069}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_GREAT_PERSON_REWARD, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.lua}}
:<code>UI/InGame/Popups/MilitaryOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0380}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_MILITARY_OVERVIEW, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NaturalWonderPopup.lua}}
:<code>UI/InGame/Popups/NaturalWonderPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0115}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_NATURAL_WONDER_REWARD, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NewEraPopup.lua}}
:<code>UI/InGame/Popups/NewEraPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0082}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_NEW_ERA, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationLogPopup.lua}}
:<code>UI/InGame/Popups/NotificationLogPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0113}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_NOTIFICATION_LOG, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1099}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_CHOOSEPRODUCTION, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetCityName.lua}}
:<code>UI/InGame/Popups/SetCityName.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_RENAME_CITY, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SetUnitName.lua}}
:<code>UI/InGame/Popups/SetUnitName.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0104}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_RENAME_UNIT, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SocialPolicyPopup.lua}}
:<code>UI/InGame/Popups/SocialPolicyPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0927}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_CHOOSEPOLICY, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechAwardPopup.lua}}
:<code>UI/InGame/Popups/TechAwardPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0134}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_TECH_AWARD, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0027}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed(ButtonPopupTypes.BUTTONPOPUP_CHOOSETECH, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0028}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed(popupType, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechTree.lua}}
:<code>UI/InGame/TechTree/TechTree.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0764}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_TECH_TREE, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TextPopup.lua}}
:<code>UI/InGame/Popups/TextPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate( ButtonPopupTypes.BUTTONPOPUP_TEXT, 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0645}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.Add(HandlePopupProcessed);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|VoteResultsPopup.lua}}
:<code>UI/InGame/Popups/VoteResultsPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0289}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_VOTE_RESULTS, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WhosWinningPopup.lua}}
:<code>UI/InGame/Popups/WhosWinningPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0332}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_WHOS_WINNING, 0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|WonderPopup.lua}}
:<code>UI/InGame/Popups/WonderPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0153}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupProcessed.CallImmediate(ButtonPopupTypes.BUTTONPOPUP_WONDER_COMPLETED_ACTIVE_PLAYER, 0);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventGameMessagePopupProcessed]]