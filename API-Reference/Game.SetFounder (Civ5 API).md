{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Game}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Game.SetFounder<b>(</b>{{Type5|ReligionType}} arg0, {{Type5|PlayerID}} newOwner<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|arg0:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|newOwner:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TurnsRemaining.lua (G&K)}}
:<code>DLC/Expansion/Scenarios/MedievalScenario/TurnsRemaining.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0205}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ORTHODOXY"], iNewOwner);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0213}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ORTHODOXY"], pNewHolyCity:GetOwner());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0223}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ISLAM"], iNewOwner);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0225}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ISLAM"], GetPersistentProperty("MeccaPlayer"));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0237}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_CHRISTIANITY"], iNewOwner);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0239}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_CHRISTIANITY"], GetPersistentProperty("VaticanPlayer"));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0251}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_PROTESTANTISM"], iNewOwner);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0253}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_PROTESTANTISM"], GetPersistentProperty("ProtestantHolyCityPlayer"));</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0339}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ISLAM"], iMeccaPlayer);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0341}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_CHRISTIANITY"], iVaticanPlayer);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0351}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_ISLAM"], iNewAlly);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0365}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_CHRISTIANITY"], iNewAlly);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0379}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_PROTESTANTISM"], iNewAlly);</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0381}}<syntaxhighlight lang="lua">Game.SetFounder(GameInfoTypes["RELIGION_PROTESTANTISM"], iProtestantPlayer);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SetFounder]]
[[Category:Civ5 Religion API|SetFounder]]