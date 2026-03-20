{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>DB.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
COLLECTMEMORYUSAGE
-->
|-
{{FuncInfos5|maybe|maybe|yes|Tells the engine to gather SQL memory usage This method tells the engine to gather extended memory information by walking the heap associated with SQL.  This method is used in conjunction with DB.GetMemoryUsage and will allow it to return more detailed information.  Each time this method is called, it updates the information snapshot returned by DB.GetMemoryUsage.  It is not recommended to execute this method on a per-frame basis as it can be quite slow.}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|DB|CollectMemoryUsage}}<!-- No arguments --></code>
<!-- 
CREATEQUERY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|DB|CreateQuery}}<b>(</b>'''string''' sql<b>)</b></code>
<!-- 
GETMEMORYUSAGE
-->
|-
{{FuncInfos5|yes  |yes  |yes|Returns the amount of memory currently in use by SQL}}
|align="right"  |<code>'''table'''</code>
|width="100%" |<code>{{FuncLabel5|DB|GetMemoryUsage}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
QUERY
-->
|-
{{FuncInfos5|yes  |yes  |yes|Executes an arbitrary SQL statement on the gameplay database and returns recordset. In situations where the quick and easy enumeration that GameInfo provides is not enough and either updates to the database or a complex query such as a join is required, DB.Query can be used.  This method executes any arbitrary SQL command on the gameplay database and returns a recordset.  Variable arguments can be used in the SQL command.  For information about how to use literal arguments, see [http://www.sqlite.org/c3ref/bind_blob.html| here]. The SQL command does not actually get executed until the query is iterated.  Even if your statement is not intended to return a record set, you must still iterate it to cause the "Step" to occur.}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|DB|Query}}<b>(</b>'''string''' SqlStatement, '''...''' statement_args = nil<b>)</b></code>
<!-- 
STATEMENTCOUNT
-->
|-
{{FuncInfos5|maybe|maybe|yes|Returns the number of active SQL commands}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|DB|StatementCount}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
STATEMENTSQL
-->
|-
{{FuncInfos5|maybe|maybe|yes|Returns the SQL string for the specified active SQL query index Used as a debug mechanism, returns the SQL text used for a specific active SQL query index.}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|DB|StatementSQL}}<b>(</b>'''int''' statement_index<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|DB]]