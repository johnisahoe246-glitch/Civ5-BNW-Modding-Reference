{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.AudioPlay2DSound<b>(</b>'''string''' audio<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.AudioPlay2DSound.Add(''<function handler>'')</code> or invoke it directly through <code>Events.AudioPlay2DSound(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|audio:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0145}}<syntaxhighlight lang="lua">Events.AudioPlay2DSound("AS2D_INTERFACE_POLICY");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1700}}<syntaxhighlight lang="lua">Events.AudioPlay2DSound("AS2D_INTERFACE_BUY_TILE");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0179}}<syntaxhighlight lang="lua">Events.AudioPlay2DSound( "AS2D_IF_MP_CHAT_DING" );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|EndGameMenu.lua}}
:<code>UI/InGame/Popups/EndGameMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0102}}<syntaxhighlight lang="lua">Events.AudioPlay2DSound(m_strAudio);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0077}}<syntaxhighlight lang="lua">Events.AudioPlay2DSound("AS2D_INTERFACE_CITY_SCREEN_PURCHASE");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ProductionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0129}}<syntaxhighlight lang="lua">Events.AudioPlay2DSound("AS2D_INTERFACE_FAITH_PURCHASE");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0802}}<syntaxhighlight lang="lua">Events.AudioPlay2DSound("AS2D_INTERFACE_UNIT_PROMOTION");</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AudioPlay2DSound]]