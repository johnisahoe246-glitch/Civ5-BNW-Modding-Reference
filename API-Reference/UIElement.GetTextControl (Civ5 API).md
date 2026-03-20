{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Function.png|This method is declared by {{Type5|Button}} and {{Type5|GridButton}}.<br/>
This is an instance method, invoke it with a colon.
}}


=Usage=
<code>{{Type5|Label}} UIElement:GetTextControl<b>(</b><b>)</b></code>


'''Returned Value'''
:No description available.


=Source code samples=
''Redundant occurences have been removed.''

{{PseudoH4|DiploCorner.lua}}
:<code>UI/InGame/WorldView/DiploCorner.lua</code>
:{{CodeBegin5}}
{{CodeLine5|0321}}<syntaxhighlight lang="lua">local textControl = controlTable.Button:GetTextControl();</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0355}}<syntaxhighlight lang="lua">textControl = controlTable.Button:GetTextControl();</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua}}
:<code>UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1008}}<syntaxhighlight lang="lua">Controls.UsPocketGold:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1011}}<syntaxhighlight lang="lua">Controls.UsPocketGold:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1023}}<syntaxhighlight lang="lua">Controls.ThemPocketGold:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1026}}<syntaxhighlight lang="lua">Controls.ThemPocketGold:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1042}}<syntaxhighlight lang="lua">Controls.UsPocketGoldPerTurn:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1045}}<syntaxhighlight lang="lua">Controls.UsPocketGoldPerTurn:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1057}}<syntaxhighlight lang="lua">Controls.ThemPocketGoldPerTurn:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1060}}<syntaxhighlight lang="lua">Controls.ThemPocketGoldPerTurn:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1083}}<syntaxhighlight lang="lua">Controls.UsPocketOpenBorders:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1091}}<syntaxhighlight lang="lua">Controls.UsPocketOpenBorders:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1101}}<syntaxhighlight lang="lua">Controls.ThemPocketOpenBorders:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1108}}<syntaxhighlight lang="lua">Controls.ThemPocketOpenBorders:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1143}}<syntaxhighlight lang="lua">Controls.UsPocketDefensivePact:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1146}}<syntaxhighlight lang="lua">Controls.UsPocketDefensivePact:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1154}}<syntaxhighlight lang="lua">Controls.ThemPocketDefensivePact:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1157}}<syntaxhighlight lang="lua">Controls.ThemPocketDefensivePact:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1198}}<syntaxhighlight lang="lua">Controls.UsPocketResearchAgreement:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1201}}<syntaxhighlight lang="lua">Controls.UsPocketResearchAgreement:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1209}}<syntaxhighlight lang="lua">Controls.ThemPocketResearchAgreement:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1212}}<syntaxhighlight lang="lua">Controls.ThemPocketResearchAgreement:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1245}}<syntaxhighlight lang="lua">Controls.UsPocketTradeAgreement:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1248}}<syntaxhighlight lang="lua">Controls.UsPocketTradeAgreement:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1256}}<syntaxhighlight lang="lua">Controls.ThemPocketTradeAgreement:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1259}}<syntaxhighlight lang="lua">Controls.ThemPocketTradeAgreement:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1276}}<syntaxhighlight lang="lua">Controls.UsPocketCities:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1280}}<syntaxhighlight lang="lua">Controls.UsPocketCities:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1294}}<syntaxhighlight lang="lua">Controls.ThemPocketCities:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1298}}<syntaxhighlight lang="lua">Controls.ThemPocketCities:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1308}}<syntaxhighlight lang="lua">Controls.UsPocketOtherPlayer:GetTextControl():SetColorByName( "Gray_Black" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1313}}<syntaxhighlight lang="lua">Controls.ThemPocketOtherPlayer:GetTextControl():SetColorByName( "Gray_Black" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1319}}<syntaxhighlight lang="lua">Controls.UsPocketOtherPlayer:GetTextControl():SetColorByName( "Beige_Black" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1324}}<syntaxhighlight lang="lua">Controls.ThemPocketOtherPlayer:GetTextControl():SetColorByName( "Beige_Black" );</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1378}}<syntaxhighlight lang="lua">Controls.UsPocketLuxury:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1386}}<syntaxhighlight lang="lua">Controls.UsPocketLuxury:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1393}}<syntaxhighlight lang="lua">Controls.UsPocketStrategic:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1401}}<syntaxhighlight lang="lua">Controls.UsPocketStrategic:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1445}}<syntaxhighlight lang="lua">Controls.ThemPocketLuxury:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1453}}<syntaxhighlight lang="lua">Controls.ThemPocketLuxury:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1460}}<syntaxhighlight lang="lua">Controls.ThemPocketStrategic:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1468}}<syntaxhighlight lang="lua">Controls.ThemPocketStrategic:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|TradeLogic.lua (G&K)}}
:<code>DLC/Expansion/UI/InGame/WorldView/TradeLogic.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1101}}<syntaxhighlight lang="lua">Controls.UsPocketAllowEmbassy:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1108}}<syntaxhighlight lang="lua">Controls.UsPocketAllowEmbassy:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1124}}<syntaxhighlight lang="lua">Controls.ThemPocketAllowEmbassy:GetTextControl(): SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1131}}<syntaxhighlight lang="lua">Controls.ThemPocketAllowEmbassy:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1370}}<syntaxhighlight lang="lua">Controls.UsPocketDoF:GetTextControl():SetColorByName("Gray_Black");</syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|1381}}<syntaxhighlight lang="lua">Controls.UsPocketDoF:GetTextControl():SetColorByName("Beige_Black");</syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UnitFlagManager.lua}}
:<code>UI/InGame/UnitFlagManager.lua</code>
:{{CodeBegin5}}
{{CodeLine5|1061}}<syntaxhighlight lang="lua">local tw, th = controlTable.Button:GetTextControl():GetSizeVal();</syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Methods and Functions|GetTextControl]]