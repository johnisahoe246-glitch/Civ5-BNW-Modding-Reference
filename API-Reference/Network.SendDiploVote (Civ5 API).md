{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendDiploVote<b>(</b>{{Type5|SpecialistType}} votePlayer<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|votePlayer:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploVotePopup.lua}}
:<code>UI/InGame/Popups/DiploVotePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0011}}<syntaxhighlight lang="lua">Network.SendDiploVote(iVotePlayer);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendDiploVote]]
[[Category:Civ5 Diplomacy API|SendDiploVote]]
[[Category:Civ5 United Nations API|SendDiploVote]]