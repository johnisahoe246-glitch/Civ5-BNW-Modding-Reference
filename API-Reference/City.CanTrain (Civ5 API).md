{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' City:CanTrain<b>(</b>{{Type5|UnitType}} unit, '''int''' continue, '''int''' testVisible, '''bool''' ignoreCost, '''bool''' ignoreUpgrades<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|unit:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|continue:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|testVisible:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ignoreCost:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|ignoreUpgrades:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ProductionPopup.lua}}
:<code>UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0271}}<syntaxhighlight lang="lua">if city:CanTrain( unitID, 0, 1 ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0274}}<syntaxhighlight lang="lua">if not city:CanTrain( unitID ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanTrain]]
[[Category:Civ5 City Production API|CanTrain]]