{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|City}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' City:GetNumThingsProduced<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|TutorialChecks.lua}}
:<code>Tutorial/TutorialChecks.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0773}}<syntaxhighlight lang="lua">if (v:GetNumThingsProduced() > 1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0775}}<syntaxhighlight lang="lua">elseif (v:GetNumThingsProduced() == 1 and result == INACTIVE) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3544}}<syntaxhighlight lang="lua">if (v:GetNumThingsProduced() > iMaxThingsCityBuilt) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|3546}}<syntaxhighlight lang="lua">iMaxThingsCityBuilt = v:GetNumThingsProduced();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumThingsProduced]]