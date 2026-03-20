{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendFoundPantheon<b>(</b>{{Type5|PlayerID}} arg0, {{Type5|BeliefType}} Belief<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|Belief:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|ChoosePantheonPopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChoosePantheonPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0144}}<syntaxhighlight lang="lua">Network.SendFoundPantheon(Game.GetActivePlayer(), g_BeliefID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendFoundPantheon]]
[[Category:Civ5 Religion API|SendFoundPantheon]]