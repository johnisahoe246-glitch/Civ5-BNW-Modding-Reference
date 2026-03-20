{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' Unit:SetDeployFromOperationTurn<b>(</b>'''int''' arg0<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua - DLC_04 DLC}}
:<code>DLC/DLC_04/Scenarios/1066Scenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0547}}<syntaxhighlight lang="lua">unit:SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0749}}<syntaxhighlight lang="lua">Map.GetPlot(42,39):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0750}}<syntaxhighlight lang="lua">Map.GetPlot(43,39):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0751}}<syntaxhighlight lang="lua">Map.GetPlot(42,38):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0752}}<syntaxhighlight lang="lua">Map.GetPlot(43,38):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0753}}<syntaxhighlight lang="lua">Map.GetPlot(44,38):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0754}}<syntaxhighlight lang="lua">Map.GetPlot(42,37):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0755}}<syntaxhighlight lang="lua">Map.GetPlot(43,37):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0756}}<syntaxhighlight lang="lua">Map.GetPlot(44,37):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0757}}<syntaxhighlight lang="lua">Map.GetPlot(45,37):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0758}}<syntaxhighlight lang="lua">Map.GetPlot(43,36):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0759}}<syntaxhighlight lang="lua">Map.GetPlot(44,36):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0760}}<syntaxhighlight lang="lua">Map.GetPlot(45,36):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0761}}<syntaxhighlight lang="lua">Map.GetPlot(43,35):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeLine5|0762}}<syntaxhighlight lang="lua">Map.GetPlot(44,35):GetUnit(0):SetDeployFromOperationTurn(1);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetDeployFromOperationTurn]]