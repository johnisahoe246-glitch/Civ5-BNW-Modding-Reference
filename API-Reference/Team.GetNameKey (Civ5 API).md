{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|Team}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>'''unknown''' Team:GetNameKey<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DeclareWarMovePopup.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/PopupsGeneric/DeclareWarMovePopup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0020}}<syntaxhighlight lang="lua">popupText = Locale.ConvertTextKey("TXT_KEY_POPUP_DOES_THIS_MEAN_WAR", Teams[eRivalTeam]:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0026}}<syntaxhighlight lang="lua">popupText = Locale.ConvertTextKey("TXT_KEY_POPUP_ENTER_CITY_STATE_WAR", Teams[eRivalTeam]:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0028}}<syntaxhighlight lang="lua">popupText = Locale.ConvertTextKey("TXT_KEY_POPUP_ENTER_LANDS_WAR", Teams[eRivalTeam]:GetNameKey());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0038}}<syntaxhighlight lang="lua">popupText = Locale.ConvertTextKey("TXT_KEY_POPUP_DOES_THIS_MEAN_WAR_PROTECTED_CITY_STATE", Teams[eRivalTeam]:GetNameKey());</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNameKey]]