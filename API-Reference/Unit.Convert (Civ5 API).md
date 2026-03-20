{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Unit}}.<br/>
This is an instance method, invoke it with a colon.
}}

Copies the attributes of one unit to another before removing the former unit. Useful for replacing units such as when upgrading. Note that this function does not create the unit to copy to, however. To do this, first use {{Func5|Player|InitUnit}}.

=Usage=
<code>'''void''' Unit:Convert<b>(</b>{{Type5|Unit}} unit<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|unit:
|valign="top"| ''The unit to be copied from and then removed.''
|}


{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|Convert]]