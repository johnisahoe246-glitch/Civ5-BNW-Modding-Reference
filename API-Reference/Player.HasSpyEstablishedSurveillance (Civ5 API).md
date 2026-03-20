{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''bool''' Player:HasSpyEstablishedSurveillance<b>(</b>'''unknown''' arg0<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|EspionageOverview.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/EspionageOverview.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0739}}<syntaxhighlight lang="lua">if (not pActivePlayer:HasSpyEstablishedSurveillance(v.AgentID)) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0753}}<syntaxhighlight lang="lua">local bViewDisabled = not pActivePlayer:HasSpyEstablishedSurveillance(v.AgentID) or v.State == "TXT_KEY_SPY_STATE_DEAD"</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|HasSpyEstablishedSurveillance]]
[[Category:Civ5 Espionnage API|HasSpyEstablishedSurveillance]]