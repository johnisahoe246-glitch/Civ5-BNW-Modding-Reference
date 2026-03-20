{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:IsBuildBlockedByFeature<b>(</b>{{Type5|BuildActionType}} build, {{Type5|FeatureType}} feature<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|build:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|feature:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1151}}<syntaxhighlight lang="lua">if (pActivePlayer:IsBuildBlockedByFeature(iBuildID, iFeature)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsBuildBlockedByFeature]]
[[Category:Civ5 Features & Natural wonders API|IsBuildBlockedByFeature]]
[[Category:Civ5 Improvements API|IsBuildBlockedByFeature]]