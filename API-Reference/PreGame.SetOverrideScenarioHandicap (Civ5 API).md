{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' PreGame.SetOverrideScenarioHandicap<b>(</b>'''bool''' arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|FoRScenarioLoadScreen.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/FallOfRomeScenario/FoRScenarioLoadScreen.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0057}}<syntaxhighlight lang="lua">PreGame.SetOverrideScenarioHandicap(true);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetOverrideScenarioHandicap]]
[[Category:Civ5 Game Settings API|SetOverrideScenarioHandicap]]