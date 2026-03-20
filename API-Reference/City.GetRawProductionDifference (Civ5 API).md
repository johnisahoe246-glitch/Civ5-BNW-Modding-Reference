{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetRawProductionDifference<b>(</b>'''bool''' arg0, '''bool''' arg1<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/SteampunkScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0237}}<syntaxhighlight lang="lua">iValue = pCity:GetRawProductionDifference(true, false);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetRawProductionDifference]]
[[Category:Civ5 City Production API|GetRawProductionDifference]]