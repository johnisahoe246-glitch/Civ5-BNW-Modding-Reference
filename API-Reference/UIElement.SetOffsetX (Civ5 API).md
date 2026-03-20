{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by '''ControlBase'''.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetOffsetX<b>(</b>'''int''' xOffset<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|xOffset:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0440}}<syntaxhighlight lang="lua">controls.NameStack:SetOffsetX( -7 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0444}}<syntaxhighlight lang="lua">controls.NameStack:SetOffsetX( -3 );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">barMarkerCtrl:SetOffsetX(xOffset);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPList.lua}}
:<code>UI/InGame/WorldView/MPList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0111}}<syntaxhighlight lang="lua">controlTable.Score:SetOffsetX(60);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0118}}<syntaxhighlight lang="lua">controlTable.Score:SetOffsetX(10);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0198}}<syntaxhighlight lang="lua">Controls.MPListScroll:SetOffsetX( 15 );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0279}}<syntaxhighlight lang="lua">teamEntry.Score:SetOffsetX(60);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0285}}<syntaxhighlight lang="lua">teamEntry.Score:SetOffsetX(10);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetOffsetX]]