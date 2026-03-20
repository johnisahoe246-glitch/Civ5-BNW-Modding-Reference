{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Unit:IsReadyToMove<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|ActionInfoPanel.lua}}
:<code>UI/InGame/WorldView/ActionInfoPanel.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0420}}<syntaxhighlight lang="lua">if (not pUnit:IsAutomated() and not pUnit:IsDelayedDeath() and pUnit:IsReadyToMove()) then</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0201}}<syntaxhighlight lang="lua">if (v:IsReadyToMove()) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|IsReadyToMove]]
[[Category:Civ5 Movement API|IsReadyToMove]]