{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a built-in global function. No <code>include</code> statement is needed.
}}


=Usage=
<code>{{Type5|Vector3}} HexToWorld<b>(</b>{{Type5|Vector2}} hexPos<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|hexPos:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|CityBannerManager.lua}}
:<code>UI/InGame/CityBannerManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0615}}<syntaxhighlight lang="lua">svStrikeButton.Anchor:SetWorldPosition( HexToWorld(hexPos) );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0638}}<syntaxhighlight lang="lua">local HexPos = HexToWorld( hexPos );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0665}}<syntaxhighlight lang="lua">local worldPos = HexToWorld( instance.Hex );</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.lua}}
:<code>UI/InGame/CityView/CityView.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1730}}<syntaxhighlight lang="lua">local worldPos = HexToWorld( hexPos );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|HexToWorld]]