{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Steam}}.<br/>
This is a static method, invoke it with a dot.
}}


Returns the Max number of save slots allowed on the Cloud


=Usage=
<code>{{Type5|SpecialistType}} Steam.GetMaxCloudSaves<b>(</b><b>)</b></code>


'''Returned Value'''
:Returns the Max number of save slots allowed on the Cloud.


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
print(Steam.GetMaxCloudSaves()); -- prints 10</syntaxhighlight>


=Source code samples=
{{PseudoH4|LoadMenu.lua}}
:<code>UI/FrontEnd/LoadMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0524}}<syntaxhighlight lang="lua">for i = 1, Steam.GetMaxCloudSaves(), 1 do</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|SaveMenu.lua}}
:<code>UI/InGame/Menus/SaveMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0011}}<syntaxhighlight lang="lua">s_maxCloudSaves = Steam.GetMaxCloudSaves();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMaxCloudSaves]]