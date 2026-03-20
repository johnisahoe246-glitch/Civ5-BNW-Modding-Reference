{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|DB}}.<br/>
This is a static method, invoke it with a dot.
}}


Tells the engine to gather SQL memory usage
This method tells the engine to gather extended memory information by walking the heap associated with SQL.  This method is used in conjunction with {{Func5|DB|GetMemoryUsage}} and will allow it to return more detailed information.  Each time this method is called, it updates the information snapshot returned by {{Func5|DB|GetMemoryUsage}}.  It is not recommended to execute this method on a per-frame basis as it can be quite slow.


=Usage=
<code>'''void''' DB.CollectMemoryUsage<b>(</b><b>)</b></code>




=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
--Gather SQL memory stats
DB.CollectMemoryUsage();
local info = DB.GetMemoryUsage();</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|CollectMemoryUsage]]