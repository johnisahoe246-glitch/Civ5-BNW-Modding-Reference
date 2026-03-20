{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetLeaderType<b>(</b>'''int''' arg0, '''int''' arg1<b>)</b></code>


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
{{PseudoH4|MedievalScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/MedievalScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0117}}<syntaxhighlight lang="lua">PreGame.SetLeaderType(12, GameInfo.Leaders["LEADER_GENGHIS_KHAN"].ID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetLeaderType]]
[[Category:Civ5 Players API|SetLeaderType]]