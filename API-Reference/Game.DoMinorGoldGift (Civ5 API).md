{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.DoMinorGoldGift<b>(</b>{{Type5|TeamID}} gold, '''int''' goldGiftSmall<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|gold:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|goldGiftSmall:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityStateDiploPopup.lua}}
:<code>UI/InGame/Popups/CityStateDiploPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0782}}<syntaxhighlight lang="lua">Game.DoMinorGoldGift(g_iMinorCivID, iGoldGiftSmall);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0789}}<syntaxhighlight lang="lua">Game.DoMinorGoldGift(g_iMinorCivID, iGoldGiftMedium);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0796}}<syntaxhighlight lang="lua">Game.DoMinorGoldGift(g_iMinorCivID, iGoldGiftLarge);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MinorCivGoldPopup.lua}}
:<code>UI/InGame/PopupsGeneric/MinorCivGoldPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">Game.DoMinorGoldGift(iMinor, iGoldGiftSmall);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0036}}<syntaxhighlight lang="lua">Game.DoMinorGoldGift(iMinor, iGoldGiftMedium);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0049}}<syntaxhighlight lang="lua">Game.DoMinorGoldGift(iMinor, iGoldGiftLarge);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DoMinorGoldGift]]
[[Category:Civ5 Gold API|DoMinorGoldGift]]
[[Category:Civ5 Diplomacy API|DoMinorGoldGift]]
[[Category:Civ5 City States API|DoMinorGoldGift]]