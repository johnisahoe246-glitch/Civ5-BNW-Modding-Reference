{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' AssignStartingPlots:DivideBritain<b>(</b>'''int''' numDivisions, '''unknown''' fertility_table, '''int''' rectangle_data_table<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|numDivisions:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|fertility_table:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|rectangle_data_table:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|Europe_Scenario.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/Europe_Scenario.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0985}}<syntaxhighlight lang="lua">self:DivideBritain(2, fert_table, rect_table)</syntaxhighlight>
{{CodeLine5|0986}}<syntaxhighlight lang="lua">--print("- British Isles defined as Regions 1 and 2.");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0988}}<syntaxhighlight lang="lua">-- Morocco and Tunisia.</syntaxhighlight>
{{CodeLine5|0989}}<syntaxhighlight lang="lua">self.inhabited_WestX = 3;</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|DivideBritain]]