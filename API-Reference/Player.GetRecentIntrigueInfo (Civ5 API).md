{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|SpecialistType}}, '''int''' Player:GetRecentIntrigueInfo<b>(</b>{{Type5|PlayerID}} aIPlayer<b>)</b></code>


'''Returned Values'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|aIPlayer:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|DiscussionDialog.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/LeaderHead/DiscussionDialog.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0637}}<syntaxhighlight lang="lua">iIntriguePlotter, iIntrigueType = pPlayer:GetRecentIntrigueInfo(g_iAIPlayer);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetRecentIntrigueInfo]]
[[Category:Civ5 Diplomacy API|GetRecentIntrigueInfo]]