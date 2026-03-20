{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Network}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''void''' Network.SendLiberateMinor<b>(</b>{{Type5|TeamID}} minor, {{Type5|TeamID}} city<b>)</b></code>


'''Parameters'''
:{|
|-
|valign="top" style="padding-right:6px;"|minor:
|valign="top"| ''No description available.''
|-
|valign="top" style="padding-right:6px;"|city:
|valign="top"| ''No description available.''
|}


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|LiberateMinorPopup.lua}}
:<code>UI/InGame/PopupsGeneric/LiberateMinorPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0019}}<syntaxhighlight lang="lua">Network.SendLiberateMinor(eMinor, iCityID);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|PuppetCityPopup.lua}}
:<code>UI/InGame/PopupsGeneric/PuppetCityPopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0046}}<syntaxhighlight lang="lua">Network.SendLiberateMinor(iLiberatedPlayer, cityID);</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|SendLiberateMinor]]
[[Category:Civ5 United Nations API|SendLiberateMinor]]
[[Category:Civ5 City States API|SendLiberateMinor]]