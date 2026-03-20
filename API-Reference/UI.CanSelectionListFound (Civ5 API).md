{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|UI}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' UI.CanSelectionListFound<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|InGame.lua}}
:<code>UI/InGame/InGame.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0811}}<syntaxhighlight lang="lua">if (UI.CanSelectionListFound() and player:GetNumCities() > 0) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0848}}<syntaxhighlight lang="lua">if (not UI.CanSelectionListFound()) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0965}}<syntaxhighlight lang="lua">UI.CanSelectionListFound() ) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0997}}<syntaxhighlight lang="lua">elseif( bDisplayCivilianYields and UI.CanSelectionListFound() ) then</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CanSelectionListFound]]