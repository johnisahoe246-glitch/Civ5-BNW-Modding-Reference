''This page is a part of the [[Civ5 Modding Tutorials]].''

The following markups can be used anytime a text is displayed by the civ5 UI, including mods description. They can be used both in XML or Lua. 


== Example ==
<pre>
Hello user. Are you?[NEWLINE]
[ICON_BULLET][COLOR_POSITIVE_TEXT]Good?[ENDCOLOR].
[ICON_BULLET][COLOR_NEGATIVE_TEXT]Evil?[ENDCOLOR].
</pre>


== Formatting markups ==
* <code>&#91;NEWLINE&#93;</code> inserts a line break.
* <code>&#91;TAB&#93;</code> inserts a tabulation.
* <code>&#91;SPACE&#93;</code> inserts a white space (useful at the beginning of a line in XML).
* <code>&#91;LINK&#93;</code> inserts a link. Example: <code>&#91;LINK=IMPROVEMENT_TRADING_POST&#93;The trading post&#91;/LINK&#93;</code>
* <code>&#91;T&#93;</code> ''doesn't seem to work''.


== Icons markups ==
The table below lists the icons markups. There is no ending markup, just insert one of those in your text to have it substituted with the corresponding icon. All icons are defined in the {{Table5|IconFontMapping|CIV5IconFontMapping}} and are 22 pixels high and wide.
{|
|-
|[[File:Civ5Icon.Alpha.png]] <code>&#91;ICON_ALPHA&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionBuddhism.png]] <code>&#91;ICON_RELIGION_BUDDHISM&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResSalt.png]] <code>&#91;ICON_RES_SALT&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Blockaded.png]] <code>&#91;ICON_BLOCKADED&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionChristianity.png]] <code>&#91;ICON_RELIGION_CHRISTIANITY&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResSheep.png]] <code>&#91;ICON_RES_SHEEP&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Bullet.png]] <code>&#91;ICON_BULLET&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionConfucianism.png]] <code>&#91;ICON_RELIGION_CONFUCIANISM&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResSilk.png]] <code>&#91;ICON_RES_SILK&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Capital.png]] <code>&#91;ICON_CAPITAL&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionHinduism.png]] <code>&#91;ICON_RELIGION_HINDUISM&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResSilver.png]] <code>&#91;ICON_RES_SILVER&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Citizen.png]] <code>&#91;ICON_CITIZEN&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionIslam.png]] <code>&#91;ICON_RELIGION_ISLAM&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResSpices.png]] <code>&#91;ICON_RES_SPICES&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.CityState.png]] <code>&#91;ICON_CITY_STATE&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionJudaism.png]] <code>&#91;ICON_RELIGION_JUDAISM&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResStone.png]] <code>&#91;ICON_RES_STONE&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Connected.png]] <code>&#91;ICON_CONNECTED&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionOrthodox.png]] <code>&#91;ICON_RELIGION_ORTHODOX&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResSugar.png]] <code>&#91;ICON_RES_SUGAR&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Culture.png]] <code>&#91;ICON_CULTURE&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionPantheon.png]] <code>&#91;ICON_RELIGION_PANTHEON&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResTruffles.png]] <code>&#91;ICON_RES_TRUFFLES&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Denounce.png]] <code>&#91;ICON_DENOUNCE&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionProtestant.png]] <code>&#91;ICON_RELIGION_PROTESTANT&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResUranium.png]] <code>&#91;ICON_RES_URANIUM&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Flower.png]] <code>&#91;ICON_FLOWER&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionShinto.png]] <code>&#91;ICON_RELIGION_SHINTO&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResWhale.png]] <code>&#91;ICON_RES_WHALE&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Food.png]] <code>&#91;ICON_FOOD&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionSikhism.png]] <code>&#91;ICON_RELIGION_SIKHISM&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResWheat.png]] <code>&#91;ICON_RES_WHEAT&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Gold.png]] <code>&#91;ICON_GOLD&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionTaoism.png]] <code>&#91;ICON_RELIGION_TAOISM&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResWine.png]] <code>&#91;ICON_RES_WINE&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.GoldenAge.png]] <code>&#91;ICON_GOLDEN_AGE&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionTengriism.png]] <code>&#91;ICON_RELIGION_TENGRIISM&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Research.png]] <code>&#91;ICON_RESEARCH&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.GreatPeople.png]] <code>&#91;ICON_GREAT_PEOPLE&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ReligionZoroastrianism.png]] <code>&#91;ICON_RELIGION_ZOROASTRIANISM&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Resistance.png]] <code>&#91;ICON_RESISTANCE&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Happiness1.png]] <code>&#91;ICON_HAPPINESS_1&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResAluminum.png]] <code>&#91;ICON_RES_ALUMINUM&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Spy.png]] <code>&#91;ICON_SPY&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Happiness2.png]] <code>&#91;ICON_HAPPINESS_2&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResBanana.png]] <code>&#91;ICON_RES_BANANA&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Star.png]] <code>&#91;ICON_STAR&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Happiness3.png]] <code>&#91;ICON_HAPPINESS_3&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResCitrus.png]] <code>&#91;ICON_RES_CITRUS&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Strength.png]] <code>&#91;ICON_STRENGTH&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Happiness4.png]] <code>&#91;ICON_HAPPINESS_4&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResCoal.png]] <code>&#91;ICON_RES_COAL&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Team1.png]] <code>&#91;ICON_TEAM_1&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Influence.png]] <code>&#91;ICON_INFLUENCE&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResCopper.png]] <code>&#91;ICON_RES_COPPER&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Team10.png]] <code>&#91;ICON_TEAM_10&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Inquisitor.png]] <code>&#91;ICON_INQUISITOR&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResCotton.png]] <code>&#91;ICON_RES_COTTON&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Team11.png]] <code>&#91;ICON_TEAM_11&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Invest.png]] <code>&#91;ICON_INVEST&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResCow.png]] <code>&#91;ICON_RES_COW&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Team2.png]] <code>&#91;ICON_TEAM_2&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Locked.png]] <code>&#91;ICON_LOCKED&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResCrab.png]] <code>&#91;ICON_RES_CRAB&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Team3.png]] <code>&#91;ICON_TEAM_3&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Minus.png]] <code>&#91;ICON_MINUS&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResDeer.png]] <code>&#91;ICON_RES_DEER&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Team4.png]] <code>&#91;ICON_TEAM_4&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Missionary.png]] <code>&#91;ICON_MISSIONARY&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResDye.png]] <code>&#91;ICON_RES_DYE&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Team5.png]] <code>&#91;ICON_TEAM_5&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Moves.png]] <code>&#91;ICON_MOVES&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResFish.png]] <code>&#91;ICON_RES_FISH&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Team6.png]] <code>&#91;ICON_TEAM_6&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Mushroom.png]] <code>&#91;ICON_MUSHROOM&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResFur.png]] <code>&#91;ICON_RES_FUR&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Team7.png]] <code>&#91;ICON_TEAM_7&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Occupied.png]] <code>&#91;ICON_OCCUPIED&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResGems.png]] <code>&#91;ICON_RES_GEMS&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Team8.png]] <code>&#91;ICON_TEAM_8&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Omega.png]] <code>&#91;ICON_OMEGA&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResGold.png]] <code>&#91;ICON_RES_GOLD&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Team9.png]] <code>&#91;ICON_TEAM_9&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Peace.png]] <code>&#91;ICON_PEACE&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResHorse.png]] <code>&#91;ICON_RES_HORSE&#93;</code>
|width="50px"|
|[[File:Civ5Icon.TeamUsa.png]] <code>&#91;ICON_TEAM_USA&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Pirate.png]] <code>&#91;ICON_PIRATE&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResIncense.png]] <code>&#91;ICON_RES_INCENSE&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Trade.png]] <code>&#91;ICON_TRADE&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Plus.png]] <code>&#91;ICON_PLUS&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResIron.png]] <code>&#91;ICON_RES_IRON&#93;</code>
|width="50px"|
|[[File:Civ5Icon.TradeWhite.png]] <code>&#91;ICON_TRADE_WHITE&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Production.png]] <code>&#91;ICON_PRODUCTION&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResIvory.png]] <code>&#91;ICON_RES_IVORY&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ViewCity.png]] <code>&#91;ICON_VIEW_CITY&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Prophet.png]] <code>&#91;ICON_PROPHET&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResJewelry.png]] <code>&#91;ICON_RES_JEWELRY&#93;</code>
|width="50px"|
|[[File:Civ5Icon.War.png]] <code>&#91;ICON_WAR&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Puppet.png]] <code>&#91;ICON_PUPPET&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResMarble.png]] <code>&#91;ICON_RES_MARBLE&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Worker.png]] <code>&#91;ICON_WORKER&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.RangeStrength.png]] <code>&#91;ICON_RANGE_STRENGTH&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResOil.png]] <code>&#91;ICON_RES_OIL&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Wtf1.png]] <code>&#91;ICON_WTF1&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Razing.png]] <code>&#91;ICON_RAZING&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResPearls.png]] <code>&#91;ICON_RES_PEARLS&#93;</code>
|width="50px"|
|[[File:Civ5Icon.Wtf2.png]] <code>&#91;ICON_WTF2&#93;</code>
|width="50px"|
|-
|[[File:Civ5Icon.Religion.png]] <code>&#91;ICON_RELIGION&#93;</code>
|width="50px"|
|[[File:Civ5Icon.ResPorcelain.png]] <code>&#91;ICON_RES_PORCELAIN&#93;</code>
|width="50px"|
|}


== Colors markups ==
The table below lists the main opening color markups (players colors have been excluded, as long as a few translucent ones). Use <code>[ENDCOLOR]</code> as the ending markup. All colors are defined in the {{Table5|Colors|CIV5Colors}} table.
:You can also use custom colors through the following syntax: <code>&#91;COLOR:255:235:0:255&#93;</code>
{|
|width="40px" style="background:#FFFF00"|
|width="0px"|
|<code> &#91;COLOR_ADVISOR_HIGHLIGHT_TEXT&#93;</code>
|width="50px"|
|width="40px" style="background:#1AF200"|
|width="0px"|
|<code> &#91;COLOR_FONT_GREEN&#93;</code>
|width="50px"|
|width="40px" style="background:#00FFFF"|
|width="0px"|
|<code> &#91;COLOR_RESEARCH_STORED&#93;</code>
|width="50px"|
|-
|width="40px" style="background:#80FF1A"|
|width="0px"|
|<code> &#91;COLOR_ALT_HIGHLIGHT_TEXT&#93;</code>
|width="50px"|
|width="40px" style="background:#FF4C26"|
|width="0px"|
|<code> &#91;COLOR_FONT_RED&#93;</code>
|width="50px"|
|width="40px" style="background:#FFD17D"|
|width="0px"|
|<code> &#91;COLOR_SELECTED_TEXT&#93;</code>
|width="50px"|
|-
|width="40px" style="background:#000000"|
|width="0px"|
|<code> &#91;COLOR_BLACK&#93;</code>
|width="50px"|
|width="40px" style="background:#FFFF00"|
|width="0px"|
|<code> &#91;COLOR_GREAT_PEOPLE_STORED&#93;</code>
|width="50px"|
|width="40px" style="background:#80FF1A"|
|width="0px"|
|<code> &#91;COLOR_TECH_TEXT&#93;</code>
|width="50px"|
|-
|width="40px" style="background:#0000FF"|
|width="0px"|
|<code> &#91;COLOR_BLUE&#93;</code>
|width="50px"|
|width="40px" style="background:#00FF00"|
|width="0px"|
|<code> &#91;COLOR_GREEN&#93;</code>
|width="50px"|
|width="40px" style="background:#FFFF00"|
|width="0px"|
|<code> &#91;COLOR_UNIT_TEXT&#93;</code>
|width="50px"|
|-
|width="40px" style="background:#663D29"|
|width="0px"|
|<code> &#91;COLOR_BROWN_TEXT&#93;</code>
|width="50px"|
|width="40px" style="background:#808080"|
|width="0px"|
|<code> &#91;COLOR_GREY&#93;</code>
|width="50px"|
|width="40px" style="background:#FF4C4C"|
|width="0px"|
|<code> &#91;COLOR_WARNING_TEXT&#93;</code>
|width="50px"|
|-
|width="40px" style="background:#CCCCD9"|
|width="0px"|
|<code> &#91;COLOR_BUILDING_TEXT&#93;</code>
|width="50px"|
|width="40px" style="background:#66E6FF"|
|width="0px"|
|<code> &#91;COLOR_HIGHLIGHT_TEXT&#93;</code>
|width="50px"|
|width="40px" style="background:#B2B2FF"|
|width="0px"|
|<code> &#91;COLOR_WATER_TEXT&#93;</code>
|width="50px"|
|-
|width="40px" style="background:#1275CC"|
|width="0px"|
|<code> &#91;COLOR_CITY_BLUE&#93;</code>
|width="50px"|
|width="40px" style="background:#BFBFBF"|
|width="0px"|
|<code> &#91;COLOR_LIGHT_GREY&#93;</code>
|width="50px"|
|width="40px" style="background:#FFFFFF"|
|width="0px"|
|<code> &#91;COLOR_WHITE&#93;</code>
|width="50px"|
|-
|width="40px" style="background:#B27300"|
|width="0px"|
|<code> &#91;COLOR_CITY_BROWN&#93;</code>
|width="50px"|
|width="40px" style="background:#FF00FF"|
|width="0px"|
|<code> &#91;COLOR_MAGENTA&#93;</code>
|width="50px"|
|width="40px" style="background:#0078FC"|
|width="0px"|
|<code> &#91;COLOR_XP_BLUE&#93;</code>
|width="50px"|
|-
|width="40px" style="background:#2E876B"|
|width="0px"|
|<code> &#91;COLOR_CITY_GREEN&#93;</code>
|width="50px"|
|width="40px" style="background:#47D4F2"|
|width="0px"|
|<code> &#91;COLOR_MENU_BLUE&#93;</code>
|width="50px"|
|width="40px" style="background:#FFFF00"|
|width="0px"|
|<code> &#91;COLOR_YELLOW&#93;</code>
|width="50px"|
|-
|width="40px" style="background:#594040"|
|width="0px"|
|<code> &#91;COLOR_CITY_GREY&#93;</code>
|width="50px"|
|width="40px" style="background:#FF4C4C"|
|width="0px"|
|<code> &#91;COLOR_NEGATIVE_TEXT&#93;</code>
|width="50px"|
|width="40px" style="background:#FC9429"|
|width="0px"|
|<code> &#91;COLOR_YIELD_FOOD&#93;</code>
|width="50px"|
|-
|width="40px" style="background:#9900FF"|
|width="0px"|
|<code> &#91;COLOR_CULTURE_STORED&#93;</code>
|width="50px"|
|width="40px" style="background:#FFFFFF"|
|width="0px"|
|<code> &#91;COLOR_POPUP_TEXT&#93;</code>
|width="50px"|
|width="40px" style="background:#FFF014"|
|width="0px"|
|<code> &#91;COLOR_YIELD_GOLD&#93;</code>
|width="50px"|
|-
|width="40px" style="background:#00FFFF"|
|width="0px"|
|<code> &#91;COLOR_CYAN&#93;</code>
|width="50px"|
|width="40px" style="background:#80FF1A"|
|width="0px"|
|<code> &#91;COLOR_POSITIVE_TEXT&#93;</code>
|width="50px"|
|width="40px" style="background:#708FBD"|
|width="0px"|
|<code> &#91;COLOR_YIELD_PRODUCTION&#93;</code>
|width="50px"|
|-
|width="40px" style="background:#404040"|
|width="0px"|
|<code> &#91;COLOR_DARK_GREY&#93;</code>
|width="50px"|
|width="40px" style="background:#CCCCD9"|
|width="0px"|
|<code> &#91;COLOR_PROJECT_TEXT&#93;</code>
|width="50px"|
|}


[[Category:Civ5 Tutorials]]