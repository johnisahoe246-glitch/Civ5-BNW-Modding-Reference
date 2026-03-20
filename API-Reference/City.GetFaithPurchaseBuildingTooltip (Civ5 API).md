{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetFaithPurchaseBuildingTooltip<b>(</b>'''int''' id<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|id:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ProductionPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ProductionPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1086}}<syntaxhighlight lang="lua">strDisabledInfo = pCity:GetFaithPurchaseBuildingTooltip(id);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetFaithPurchaseBuildingTooltip]]
[[Category:Civ5 City Production API|GetFaithPurchaseBuildingTooltip]]
[[Category:Civ5 Buildings API|GetFaithPurchaseBuildingTooltip]]
[[Category:Civ5 Religion API|GetFaithPurchaseBuildingTooltip]]