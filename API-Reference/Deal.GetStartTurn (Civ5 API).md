{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Deal}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Deal:GetStartTurn<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
{{PseudoH4|DiploCurrentDeals.lua}}
:<code>UI/InGame/Popups/DiploCurrentDeals.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0089}}<syntaxhighlight lang="lua">controlTable.TurnsLabel:LocalizeAndSetText( "TXT_KEY_DO_ON_TURN", m_Deal:GetStartTurn() );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0146}}<syntaxhighlight lang="lua">local iBeginTurn = m_Deal:GetStartTurn();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetStartTurn]]