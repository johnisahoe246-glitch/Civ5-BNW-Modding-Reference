{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:GetNumResourceNeededToUpgrade<b>(</b>{{Type5|ResourceType}} resourceLoop<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|resourceLoop:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|UnitPanel.lua}}
:<code>UI/InGame/WorldView/UnitPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0992}}<syntaxhighlight lang="lua">iNumResourceNeededToUpgrade = unit:GetNumResourceNeededToUpgrade(iResourceLoop);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumResourceNeededToUpgrade]]
[[Category:Civ5 Resources API|GetNumResourceNeededToUpgrade]]
[[Category:Civ5 Units API|GetNumResourceNeededToUpgrade]]