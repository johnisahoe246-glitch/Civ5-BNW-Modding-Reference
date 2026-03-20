{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>ReligionType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>ReligionType</code> corresponds to the ''ID'' column of the {{Table5|Religions|CIV5Religions}} XML table.
* {{Lua}} The standard (unmodded) values in the ''ID'' and ''Type'' columns are also stored in the '''ReligionTypes''' Lua enumeration.
}}


= Lua: the ReligionTypes enumeration =
Firaxis provides a Lua enumeration named <code>ReligionTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.
* This specific enumeration contains data from the {{Table5|Religions|CIV5Religions}} data table.<br/>
* They are stored as key/value pairs: the keys are the strings from the ''Type'' column and the values are the integers from the ''ID'' column.<br/>
{{Warning}} Be careful: this enumeration do '''not''' reflect the changes, additions and deletions made by mods. As a result it is advised to rely on {{Type5|GameInfo}} instead.<br/>

<br/>Below are the values found in this enumeration.
<code>
{|
|-
!align="left" |Key
!
!align="left" |Value 
|-
|align="left" |"NO_RELIGION"
|
|align="right" |-1
|-
|align="left" |"RELIGION_PANTHEON"
|
|align="right" |0
|}</code>


= XML: the Religions table =
Here are the ''ID'' and ''Type'' columns found in this table.
<code>
{|
|-
!align="left" |ID
!
!align="left" |Type
|-
|align="right"|0
|
|RELIGION_PANTHEON
|-
|align="right"|1
|
|RELIGION_BUDDHISM
|-
|align="right"|2
|
|RELIGION_CHRISTIANITY
|-
|align="right"|3
|
|RELIGION_CONFUCIANISM
|-
|align="right"|4
|
|RELIGION_HINDUISM
|-
|align="right"|5
|
|RELIGION_ISLAM
|-
|align="right"|6
|
|RELIGION_JUDAISM
|-
|align="right"|7
|
|RELIGION_SHINTO
|-
|align="right"|8
|
|RELIGION_SIKHISM
|-
|align="right"|9
|
|RELIGION_TAOISM
|-
|align="right"|10
|
|RELIGION_TENGRIISM
|-
|align="right"|11
|
|RELIGION_ZOROASTRIANISM
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0.
<syntaxhighlight lang="lua" class="civ5-example">
local id = ReligionTypes.RELIGION_PANTHEON
local id = ReligionTypes["RELIGION_PANTHEON"]
</syntaxhighlight>
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Religions.RELIGION_PANTHEON.ID
local id = GameInfo["Religions"].["RELIGION_PANTHEON"].ID
local id = GameInfo.Religions{Type="RELIGION_PANTHEON"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_RELIGION_PANTHEON.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Religions[0].Description
local description = GameInfo["Religions"][0]["Description"]
local description = GameInfo.Religions{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
ADOPTRELIGIONFULLY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|AdoptReligionFully}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
CONVERTPERCENTFOLLOWERS
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|ConvertPercentFollowers}}<b>(</b>{{Type5|ReligionType}} arg0, {{Type5|ReligionType}} arg1, '''int''' arg2<b>)</b></code>
<!-- 
GETNUMFOLLOWERS
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetNumFollowers}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
GETPRESSUREPERTURN
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetPressurePerTurn}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
GETRELIGIOUSMAJORITY
-->
|-
|align="right" width="200" |<code>{{Type5|ReligionType}}</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|GetReligiousMajority}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISHOLYCITYFORRELIGION
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|City}}:{{Func5|City|IsHolyCityForReligion}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
ENHANCERELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|EnhanceReligion}}<b>(</b>{{Type5|PlayerID}} vaticanPlayer, {{Type5|ReligionType}} religion, {{Type5|BeliefType}} belief4, {{Type5|BeliefType}} belief5<b>)</b></code>
<!-- 
FOUNDRELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|FoundReligion}}<b>(</b>{{Type5|PlayerID}} vaticanPlayer, {{Type5|ReligionType}} religion, '''unknown''' arg2, {{Type5|BeliefType}} belief2, {{Type5|BeliefType}} belief3, {{Type5|BeliefType}} belief3, '''int''' arg6, {{Type5|City}} vaticanCity<b>)</b></code>
<!-- 
GETFOUNDER
-->
|-
|align="right" width="200" |<code>{{Type5|PlayerID}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetFounder}}<b>(</b>{{Type5|ReligionType}} arg0, '''int''' arg1<b>)</b></code>
<!-- 
GETFOUNDERBENEFITSRELIGION
-->
|-
|align="right" width="200" |<code>{{Type5|ReligionType}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetFounderBenefitsReligion}}<b>(</b>{{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETHOLYCITYFORRELIGION
-->
|-
|align="right" width="200" |<code>{{Type5|City}}</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetHolyCityForReligion}}<b>(</b>{{Type5|ReligionType}} religion, {{Type5|PlayerID}} player<b>)</b></code>
<!-- 
GETNUMCITIESFOLLOWING
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetNumCitiesFollowing}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
GETRELIGIONNAME
-->
|-
|align="right" width="200" |<code>'''string'''</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetReligionName}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
SETFOUNDER
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetFounder}}<b>(</b>{{Type5|ReligionType}} arg0, {{Type5|PlayerID}} newOwner<b>)</b></code>
<!-- 
SETHOLYCITY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|SetHolyCity}}<b>(</b>{{Type5|ReligionType}} arg0, {{Type5|City}} newHolyCity<b>)</b></code>
<!-- 
CITYCONVERTSRELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GameEvents}}.{{Func5|GameEvents|CityConvertsReligion}}<b>(</b>{{Type5|PlayerID}} owner, {{Type5|ReligionType}} religion, '''int''' x, '''int''' y<b>)</b></code>
<!-- 
SENDENHANCERELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendEnhanceReligion}}<b>(</b>{{Type5|PlayerID}} arg0, {{Type5|ReligionType}} CurrentReligion, '''unknown''' customName, '''unknown''' arg3, '''int''' arg4, '''int''' cityX, '''int''' cityY<b>)</b></code>
<!-- 
SENDFOUNDRELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendFoundReligion}}<b>(</b>{{Type5|PlayerID}} arg0, {{Type5|ReligionType}} CurrentReligion, '''unknown''' customName, '''unknown''' arg3, '''unknown''' arg4, {{Type5|BeliefType}} arg5, {{Type5|BeliefType}} arg6, '''int''' cityX, '''int''' cityY<b>)</b></code>
<!-- 
GETRELIGIONCREATEDBYPLAYER
-->
|-
|align="right" width="200" |<code>{{Type5|ReligionType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetReligionCreatedByPlayer}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
HASRELIGIONINMOSTCITIES
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|HasReligionInMostCities}}<b>(</b>{{Type5|ReligionType}} religion<b>)</b></code>
<!-- 
GETMAJORITYRELIGIONAFTERSPREAD
-->
|-
|align="right" width="200" |<code>{{Type5|ReligionType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetMajorityReligionAfterSpread}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETRELIGION
-->
|-
|align="right" width="200" |<code>{{Type5|ReligionType}}</code>
|style="padding-left:6px" |<code>{{Type5|Unit}}:{{Func5|Unit|GetReligion}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|ReligionType]]