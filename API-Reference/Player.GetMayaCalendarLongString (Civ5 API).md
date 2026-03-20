{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''string''' Player:GetMayaCalendarLongString<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TopPanel.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/TopPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0246}}<syntaxhighlight lang="lua">local toolTipString = Locale.ConvertTextKey("TXT_KEY_MAYA_DATE_TOOLTIP", pPlayer:GetMayaCalendarLongString(), traditionalDate);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMayaCalendarLongString]]
[[Category:Civ5 Turns API|GetMayaCalendarLongString]]