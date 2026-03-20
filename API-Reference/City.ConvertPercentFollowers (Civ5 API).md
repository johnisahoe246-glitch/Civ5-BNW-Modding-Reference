{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' City:ConvertPercentFollowers<b>(</b>{{Type5|ReligionType}} arg0, {{Type5|ReligionType}} arg1, '''int''' arg2<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg1:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|arg2:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1588}}<syntaxhighlight lang="lua">pCity:ConvertPercentFollowers(GameInfoTypes["RELIGION_PROTESTANTISM"], GameInfoTypes["RELIGION_CHRISTIANITY"], 40);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|ConvertPercentFollowers]]