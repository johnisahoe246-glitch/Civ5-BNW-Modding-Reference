{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|AssignStartingPlots}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''' AssignStartingPlots:GetWorldLuxuryTargetNumbers<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AssignStartingPlots.lua (G&K)}}
:<code>DLC/Expansion/Gameplay/Lua/AssignStartingPlots.lua</code>
:{{CodeBegin5}}
{{CodeLine5|8750}}<syntaxhighlight lang="lua">local world_size_data = self:GetWorldLuxuryTargetNumbers()</syntaxhighlight>
{{CodeLine5|8751}}<syntaxhighlight lang="lua">local targetLuxForThisWorldSize = world_size_data[1];</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetWorldLuxuryTargetNumbers]]
[[Category:Civ5 Combat API|GetWorldLuxuryTargetNumbers]]