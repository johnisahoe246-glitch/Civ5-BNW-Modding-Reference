{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of ControlBase.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetScrollValue<b>(</b>'''int''' arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChooseReligionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0533}}<syntaxhighlight lang="lua">Controls.BeliefScrollPanel:SetScrollValue(0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|6116}}<syntaxhighlight lang="lua">Controls.ScrollPanel:SetScrollValue( 0 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0183}}<syntaxhighlight lang="lua">Controls.ChatScroll:SetScrollValue( 1 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InstalledPanel.lua}}
:<code>UI/FrontEnd/Modding/InstalledPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0752}}<syntaxhighlight lang="lua">Controls.DescriptionScrollPanel:SetScrollValue(0);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0454}}<syntaxhighlight lang="lua">Controls.UsPocketPanel:SetScrollValue( 0 );</syntaxhighlight>
{{CodeLine5|0455}}<syntaxhighlight lang="lua">Controls.UsTablePanel:SetScrollValue( 0 );</syntaxhighlight>
{{CodeLine5|0456}}<syntaxhighlight lang="lua">Controls.ThemPocketPanel:SetScrollValue( 0 );</syntaxhighlight>
{{CodeLine5|0457}}<syntaxhighlight lang="lua">Controls.ThemTablePanel:SetScrollValue( 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2497}}<syntaxhighlight lang="lua">m_panel:SetScrollValue( 0 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|2636}}<syntaxhighlight lang="lua">panel:SetScrollValue( 0 );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetScrollValue]]