{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.SerialEventGameMessagePopupShown<b>(</b>{{Type5|PopupInfo}} PopupInfo<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.SerialEventGameMessagePopupShown.Add(''<function handler>'')</code> or invoke it directly through <code>Events.SerialEventGameMessagePopupShown(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|PopupInfo:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvisorCounselPopup.lua}}
:<code>UI/InGame/Popups/AdvisorCounselPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0305}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupShown(m_PopupInfo);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0165}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupShown(g_PopupInfo);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TechPopup.lua}}
:<code>UI/InGame/TechPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0072}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupShown(popupInfo);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialEngine.lua}}
:<code>Tutorial/TutorialEngine.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0644}}<syntaxhighlight lang="lua">Events.SerialEventGameMessagePopupShown.Add(HandlePopupShown);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SerialEventGameMessagePopupShown]]