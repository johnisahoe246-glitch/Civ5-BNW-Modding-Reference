{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|DB}}.<br/>
This is a static method, invoke it with a dot.
}}


Returns the SQL string for the specified active SQL query index
Used as a debug mechanism, returns the SQL text used for a specific active SQL query index.


=Usage=
<code>'''string''' DB.StatementSQL<b>(</b>'''int''' statement_index<b>)</b></code>


'''Returned Value'''
:The SQL string for an active command or nil.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|statement_index:
|valign="top"| ''A 0-based index for the current active SQL commands.  Use {{Func5|DB|StatementCount}} to obtain the number of active commands.''
|}


=Examples=
<syntaxhighlight lang="lua" class="civ5-example">
-- Print all active SQL statements.
for idx = 0, DB.StatementCount() - 1, 1 do
print(DB.StatementSQL(idx);
end</syntaxhighlight>


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|StatementSQL]]