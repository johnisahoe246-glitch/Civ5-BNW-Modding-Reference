{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Unit:IsHasPromotion<b>(</b>{{Type5|PromotionType}} promotion<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|promotion:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|EnemyUnitPanel.lua}}
:<code>UI/InGame/WorldView/EnemyUnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0140}}<syntaxhighlight lang="lua">if(pUnit:IsHasPromotion(unitPromotionID)) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0548}}<syntaxhighlight lang="lua">if (unit:IsHasPromotion(unitPromotionID)) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsHasPromotion]]
[[Category:Civ5 Unit Experience API|IsHasPromotion]]