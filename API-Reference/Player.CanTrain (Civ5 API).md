{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:CanTrain<b>(</b>{{Type5|UnitType}} unit, '''bool''' continue, '''bool''' testVisible, '''bool''' arg3, '''bool''' arg4<b>)</b></code>


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
|valign="top" style="padding-right:6px;"|arg3:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg4:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ChooseFaithGreatPerson.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseFaithGreatPerson.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0028}}<syntaxhighlight lang="lua">if(player:CanTrain(info.ID, true, true, true, false)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseFreeItem.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseFreeItem.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0028}}<syntaxhighlight lang="lua">if(player:CanTrain(info.ID, true, true, true, false) and</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanTrain]]
[[Category:Civ5 City Production API|CanTrain]]