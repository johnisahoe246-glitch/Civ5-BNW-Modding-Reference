{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Events}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Events.TaskListUpdate<b>(</b>{{Type5|PopupInfo}} TaskListInfo<b>)</b></code>


'''Event Type'''
:Regular event: you can subscribe to it through <code>Events.TaskListUpdate.Add(''<function handler>'')</code> or invoke it directly through <code>Events.TaskListUpdate(''<arguments list>'')</code>.

'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|TaskListInfo:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|TaskList.lua}}
:<code>UI/InGame/TaskList.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">Events.TaskListUpdate.Add( OnUpdate );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|TaskListUpdate]]