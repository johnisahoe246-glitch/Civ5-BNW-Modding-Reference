{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This function is a member of {{Type5|PreGame}}.<br/>
This is a static method, invoke it with a dot.
}}


=Usage=
<code>'''int''' PreGame.GetNumMinorCivs<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|AdvancedSetup.lua}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0945}}<syntaxhighlight lang="lua">if (PreGame.GetNumMinorCivs() == -1) then</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0948}}<syntaxhighlight lang="lua">Controls.MinorCivsSlider:SetValue( PreGame.GetNumMinorCivs() / maxMinorCivs );</syntaxhighlight>
{{CodeLine5|0949}}<syntaxhighlight lang="lua">Controls.MinorCivsLabel:LocalizeAndSetText("TXT_KEY_AD_SETUP_CITY_STATES", PreGame.GetNumMinorCivs());</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0958}}<syntaxhighlight lang="lua">Controls.MinorCivsSlider:SetValue(PreGame.GetNumMinorCivs() / maxMinorCivs);</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MPGameOptions.lua}}
:<code>UI/FrontEnd/Multiplayer/GameSetup/MPGameOptions.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0327}}<syntaxhighlight lang="lua">Controls.MinorCivsSlider:SetValue( PreGame.GetNumMinorCivs() / #GameInfo.MinorCivilizations );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0467}}<syntaxhighlight lang="lua">Controls.MinorCivsLabel:SetText(  Locale.ConvertTextKey("TXT_KEY_AD_SETUP_CITY_STATES", PreGame.GetNumMinorCivs()) );</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetNumMinorCivs]]
[[Category:Civ5 Players API|GetNumMinorCivs]]
[[Category:Civ5 City States API|GetNumMinorCivs]]