{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' UI.AddPopup<b>(</b>'''table''' popupInfo<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|popupInfo:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivsAlive.lua - DLC_01 DLC}}
:<code>DLC/DLC_01/Scenarios/Mongol Scenario/CivsAlive.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0128}}<syntaxhighlight lang="lua">UI.AddPopup(popupInfo);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0164}}<syntaxhighlight lang="lua">UI.AddPopup( { Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0165}}<syntaxhighlight lang="lua">Data1 = 800,</syntaxhighlight>
{{CodeLine5|0166}}<syntaxhighlight lang="lua">Option1 = true,</syntaxhighlight>
{{CodeLine5|0167}}<syntaxhighlight lang="lua">Text = "TXT_KEY_MONGOL_SCENARIO_CIV5_DAWN_MONGOLIA_TEXT" } );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_02 DLC}}
:<code>DLC/DLC_02/Scenarios/NewWorldScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0032}}<syntaxhighlight lang="lua">UI.AddPopup( { Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0033}}<syntaxhighlight lang="lua">Data1 = 800,</syntaxhighlight>
{{CodeLine5|0034}}<syntaxhighlight lang="lua">Option1 = true,</syntaxhighlight>
{{CodeLine5|0035}}<syntaxhighlight lang="lua">Text = "TXT_KEY_NEWWORLD_SCENARIO_CIV5_DAWN_NEWWORLD_TEXT" } );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">UI.AddPopup( { Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0058}}<syntaxhighlight lang="lua">Data1 = 800,</syntaxhighlight>
{{CodeLine5|0059}}<syntaxhighlight lang="lua">Option1 = true,</syntaxhighlight>
{{CodeLine5|0060}}<syntaxhighlight lang="lua">Text = "TXT_KEY_1066_SCENARIO_CIV5_DAWN_VIKING_TEXT" } );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">UI.AddPopup( { Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0058}}<syntaxhighlight lang="lua">Data1 = 800,</syntaxhighlight>
{{CodeLine5|0059}}<syntaxhighlight lang="lua">Option1 = true,</syntaxhighlight>
{{CodeLine5|0060}}<syntaxhighlight lang="lua">Text = "TXT_KEY_FOR_SCENARIO_CIV5_DAWN_TEXT" } );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0122}}<syntaxhighlight lang="lua">UI.AddPopup( { Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0123}}<syntaxhighlight lang="lua">Data1 = 800,</syntaxhighlight>
{{CodeLine5|0124}}<syntaxhighlight lang="lua">Option1 = true,</syntaxhighlight>
{{CodeLine5|0125}}<syntaxhighlight lang="lua">Text = "TXT_KEY_MEDIEVAL_SCENARIO_CIV5_DAWN_TEXT" } );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0593}}<syntaxhighlight lang="lua">UI.AddPopup( { Type = ButtonPopupTypes.BUTTONPOPUP_TEXT,</syntaxhighlight>
{{CodeLine5|0594}}<syntaxhighlight lang="lua">Data1 = 800,</syntaxhighlight>
{{CodeLine5|0595}}<syntaxhighlight lang="lua">Option1 = true,</syntaxhighlight>
{{CodeLine5|0596}}<syntaxhighlight lang="lua">Text = "TXT_KEY_STEAMPUNK_SCENARIO_CIV5_DAWN_TEXT" } );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AddPopup]]