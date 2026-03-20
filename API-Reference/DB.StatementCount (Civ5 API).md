{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|DB}}.<br/>
This is a static method, invoke it with a dot.
}}


Returns the number of active SQL commands


=Usage=
<code>'''int''' DB.StatementCount<b>(</b><b>)</b></code>


'''Returned Value'''
:The number of active SQL commands.  This is for the entire gameplay database and not just this particular Lua thread.


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
local count = DB.StatementCount();
print("Number of SQL Statements: " .. count);</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|StatementCount]]