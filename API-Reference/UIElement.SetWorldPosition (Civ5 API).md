{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|WorldAnchor}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' UIElement:SetWorldPosition<b>(</b>{{Type5|Vector3}} worldPos<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|worldPos:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0615}}<syntaxhighlight lang="lua">svStrikeButton.Anchor:SetWorldPosition( HexToWorld(hexPos) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0639}}<syntaxhighlight lang="lua">controlTable.Anchor:SetWorldPosition( VecAdd( HexPos, WorldPositionOffset ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0719}}<syntaxhighlight lang="lua">svStrikeButton.Anchor:SetWorldPosition( worldPos );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0727}}<syntaxhighlight lang="lua">controlTable.Anchor:SetWorldPosition( VecAdd( worldPos, WorldPositionOffset ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1735}}<syntaxhighlight lang="lua">controlTable.PlotButtonAnchor:SetWorldPosition( VecAdd( worldPos, WorldPositionOffset ) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1840}}<syntaxhighlight lang="lua">controlTable.BuyPlotButtonAnchor:SetWorldPosition( VecAdd( worldPos, WorldPositionOffset2 ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0914}}<syntaxhighlight lang="lua">instance.Anchor:SetWorldPosition( worldPosition );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1043}}<syntaxhighlight lang="lua">cityFlagInstance.Anchor:SetWorldPosition( VecAdd( worldPos, CityWorldPositionOffset ) );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitMemberOverlay.lua}}
:<code>UI/InGame/UnitMemberOverlay.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0207}}<syntaxhighlight lang="lua">self.m_Instance.Anchor:SetWorldPosition( position );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetWorldPosition]]