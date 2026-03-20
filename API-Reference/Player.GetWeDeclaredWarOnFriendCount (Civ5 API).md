{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetWeDeclaredWarOnFriendCount<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|InfoTooltipInclude.lua}}
:<code>UI/InGame/InfoTooltipInclude.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0804}}<syntaxhighlight lang="lua">if (pActivePlayer:GetWeDeclaredWarOnFriendCount() > 0) then      -- Human declared war on friends</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetWeDeclaredWarOnFriendCount]]
[[Category:Civ5 Diplomacy API|GetWeDeclaredWarOnFriendCount]]