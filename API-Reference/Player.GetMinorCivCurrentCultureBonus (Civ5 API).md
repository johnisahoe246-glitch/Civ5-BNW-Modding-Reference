{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Player}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''int''' Player:GetMinorCivCurrentCultureBonus<b>(</b>{{Type5|PlayerID}} major<b>)</b></code>


'''Returned Value'''
:No description available.
'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|major:
|valign="top"| ''No description available.''
|}


=Source code samples=
{{PseudoH4|CityStateStatusHelper.lua (G&K)}}
:<code>DLC/Expansion/UI/CityStateStatusHelper.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0320}}<syntaxhighlight lang="lua">local iCultureBonus = pMinor:GetMinorCivCurrentCultureBonus(iMajor);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetMinorCivCurrentCultureBonus]]
[[Category:Civ5 Culture API|GetMinorCivCurrentCultureBonus]]
[[Category:Civ5 City States API|GetMinorCivCurrentCultureBonus]]