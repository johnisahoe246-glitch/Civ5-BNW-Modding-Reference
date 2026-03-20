{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Modding}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>table('''unknown''' => '''unknown''') Modding.GetEnabledModsByActivationOrder<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|ModsMenu.lua}}
:<code>UI/FrontEnd/Modding/ModsMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0054}}<syntaxhighlight lang="lua">local mods = Modding.GetEnabledModsByActivationOrder();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetEnabledModsByActivationOrder]]