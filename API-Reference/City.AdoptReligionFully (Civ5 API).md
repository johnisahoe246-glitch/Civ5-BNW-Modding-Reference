{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''void''' City:AdoptReligionFully<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|religion:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0891}}<syntaxhighlight lang="lua">capital:AdoptReligionFully(GameInfoTypes["RELIGION_CHRISTIANITY"]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0905}}<syntaxhighlight lang="lua">capital:AdoptReligionFully(GameInfoTypes["RELIGION_ORTHODOXY"]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0907}}<syntaxhighlight lang="lua">capital:AdoptReligionFully(GameInfoTypes["RELIGION_ISLAM"]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0927}}<syntaxhighlight lang="lua">pCity:AdoptReligionFully(GameInfoTypes["RELIGION_CHRISTIANITY"]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0941}}<syntaxhighlight lang="lua">pCity:AdoptReligionFully(GameInfoTypes["RELIGION_ORTHODOXY"]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0945}}<syntaxhighlight lang="lua">pCity:AdoptReligionFully(GameInfoTypes["RELIGION_ISLAM"]);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1482}}<syntaxhighlight lang="lua">pBestCity:AdoptReligionFully(eReligion);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1500}}<syntaxhighlight lang="lua">pBestCity:AdoptReligionFully(GameInfoTypes["RELIGION_PROTESTANTISM"]);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|AdoptReligionFully]]
[[Category:Civ5 Religion API|AdoptReligionFully]]