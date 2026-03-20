{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetToolTipCallback<b>(</b>('''void''' func<b>(</b>{{Type5|Slider}} control<b>)</b>) TipHandler<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|TipHandler:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CivilopediaScreen.lua}}
:<code>UI/Civilopedia/CivilopediaScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|4623}}<syntaxhighlight lang="lua">thisListInstance.ListItemButton:SetToolTipCallback( TipHandler );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4656}}<syntaxhighlight lang="lua">thisListInstance.ListItemButton:SetToolTipCallback( TipHandler )</syntaxhighlight>
{{CodeLine5|4657}}<syntaxhighlight lang="lua">otherSortedList[tostring( thisListInstance.ListItemButton )] = sortOrder;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|4684}}<syntaxhighlight lang="lua">thisTechInstance.ListItemButton:SetToolTipCallback( TipHandler );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5520}}<syntaxhighlight lang="lua">thisTechInstance.ListItemButton:SetToolTipCallback( TipHandler )</syntaxhighlight>
{{CodeLine5|5521}}<syntaxhighlight lang="lua">otherSortedList[tostring( thisTechInstance.ListItemButton )] = sortOrder;</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|5575}}<syntaxhighlight lang="lua">thisUnitInstance.ListItemButton:SetToolTipCallback( TipHandler )</syntaxhighlight>
{{CodeLine5|5576}}<syntaxhighlight lang="lua">otherSortedList[tostring( thisUnitInstance.ListItemButton )] = sortOrder;</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua}}
:<code>UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0295}}<syntaxhighlight lang="lua">Controls.SciencePerTurn:SetToolTipCallback( ScienceTipHandler );</syntaxhighlight>
{{CodeLine5|0296}}<syntaxhighlight lang="lua">Controls.GoldPerTurn:SetToolTipCallback( GoldTipHandler );</syntaxhighlight>
{{CodeLine5|0297}}<syntaxhighlight lang="lua">Controls.HappinessString:SetToolTipCallback( HappinessTipHandler );</syntaxhighlight>
{{CodeLine5|0298}}<syntaxhighlight lang="lua">Controls.GoldenAgeString:SetToolTipCallback( GoldenAgeTipHandler );</syntaxhighlight>
{{CodeLine5|0299}}<syntaxhighlight lang="lua">Controls.CultureString:SetToolTipCallback( CultureTipHandler );</syntaxhighlight>
{{CodeLine5|0300}}<syntaxhighlight lang="lua">Controls.ResourceString:SetToolTipCallback( ResourcesTipHandler );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0331}}<syntaxhighlight lang="lua">Controls.FaithString:SetToolTipCallback( FaithTipHandler );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0244}}<syntaxhighlight lang="lua">Controls.RecommendedActionButton:SetToolTipCallback( TipHandler );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0275}}<syntaxhighlight lang="lua">instance.UnitActionButton:SetToolTipCallback( TipHandler )</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0277}}<syntaxhighlight lang="lua">end</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetToolTipCallback]]