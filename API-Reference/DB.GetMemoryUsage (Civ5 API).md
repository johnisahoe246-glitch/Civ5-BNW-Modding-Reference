{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|DB}}.<br/>
This is a static method, invoke it with a dot.
}}


Returns the amount of memory currently in use by SQL


=Usage=
<code>'''table''' DB.GetMemoryUsage<b>(</b><b>)</b></code>


'''Returned Value'''
:Returns a table with the following fields:
::NumRegions
:The number of regions in memory used by the memory manager.
::MaxUserAllocatedBytes
:The highest amount, in bytes, of allocated space requested by the application.
:''Does not require {{Func5|DB|CollectMemoryUsage}}.
::CurrentUserAllocatedBytes
:The current amount, in bytes, of allocated space requested by the application from the memory manager.
:''Does not require {{Func5|DB|CollectMemoryUsage}}.
::CurrentAllocatedBytes
:The current amount, in bytes, of allocated space used by the memory manager.
::CurrentReservedBytes
:The total amount, in bytes, of reserved memory used by the memory manager.
::CurrentOverheadBytes
:The amount, in bytes, of the overhead used by the memory manager.
::CurrentUncommitedBytes
:The amount, in bytes, of the reserved space which has not been used.


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
DB.CollectMemoryUsage();
local usage = DB.GetMemoryUsage();
print("SQL is using " .. usage.NumRegions .. " blocks of memory right now.");</syntaxhighlight>


=Source code samples=
{{PseudoH4|DebugMenu.lua}}
:<code>UI/InGame/DebugMenu.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0284}}<syntaxhighlight lang="lua">local dbmemory = DB.GetMemoryUsage();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMemoryUsage]]