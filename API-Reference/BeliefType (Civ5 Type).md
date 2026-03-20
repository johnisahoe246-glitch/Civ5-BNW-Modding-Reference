{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>BeliefType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>BeliefType</code> corresponds to the ''ID'' column of the {{Table5|Beliefs|CIV5Beliefs}} XML table.
* {{Lua}} The standard (unmodded) values in the ''ID'' and ''Type'' columns are also stored in the '''BeliefTypes''' Lua enumeration.
}}


= Lua: the BeliefTypes enumeration =
Firaxis provides a Lua enumeration named <code>BeliefTypes</code>. This is just a regular global table. Its keys are the constants' names and the pairs the corresponding values.
* This specific enumeration contains data from the {{Table5|Beliefs|CIV5Beliefs}} data table.<br/>
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
|align="left" |"NO_BELIEF"
|
|align="right" |-1
|}</code>


= XML: the Beliefs table =
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
|BELIEF_GODDESS_HUNT
|-
|align="right"|1
|
|BELIEF_FERTILITY_RITES
|-
|align="right"|2
|
|BELIEF_GOD_CRAFTSMEN
|-
|align="right"|3
|
|BELIEF_GOD_SEA
|-
|align="right"|4
|
|BELIEF_OPEN_SKY
|-
|align="right"|5
|
|BELIEF_MESSENGER_GODS
|-
|align="right"|6
|
|BELIEF_ONE_WITH_NATURE
|-
|align="right"|7
|
|BELIEF_FEED_WORLD
|-
|align="right"|8
|
|BELIEF_FORMAL_LITURGY
|-
|align="right"|9
|
|BELIEF_STONE_CIRCLES
|-
|align="right"|10
|
|BELIEF_GOD_WAR
|-
|align="right"|11
|
|BELIEF_SWORD_PLOWSHARES
|-
|align="right"|12
|
|BELIEF_GURUSHIP
|-
|align="right"|13
|
|BELIEF_HOLY_WARRIORS
|-
|align="right"|14
|
|BELIEF_SACRED_WATERS
|-
|align="right"|15
|
|BELIEF_GODDESS_LOVE
|-
|align="right"|16
|
|BELIEF_RELIGIOUS_SETTLEMENTS
|-
|align="right"|17
|
|BELIEF_GOD_FESTIVALS
|-
|align="right"|18
|
|BELIEF_ORAL_TRADITION
|-
|align="right"|19
|
|BELIEF_ANCESTOR_WORSHIP
|-
|align="right"|20
|
|BELIEF_DESERT_FOLKLORE
|-
|align="right"|21
|
|BELIEF_SACRED_PATH
|-
|align="right"|22
|
|BELIEF_GODDESS_STRATEGY
|-
|align="right"|23
|
|BELIEF_FAITH_HEALERS
|-
|align="right"|24
|
|BELIEF_MONUMENT_GODS
|-
|align="right"|25
|
|BELIEF_RELIGIOUS_TEXTS
|-
|align="right"|26
|
|BELIEF_RELIQUARY
|-
|align="right"|27
|
|BELIEF_PEACE_LOVING
|-
|align="right"|28
|
|BELIEF_INTERFAITH_DIALOGUE
|-
|align="right"|29
|
|BELIEF_CEREMONIAL_BURIAL
|-
|align="right"|30
|
|BELIEF_CHURCH_PROPERTY
|-
|align="right"|31
|
|BELIEF_TITHE
|-
|align="right"|32
|
|BELIEF_INITIATION_RITES
|-
|align="right"|33
|
|BELIEF_JUST_WAR
|-
|align="right"|34
|
|BELIEF_DEFENDER_FAITH
|-
|align="right"|35
|
|BELIEF_ITINERANT_PREACHERS
|-
|align="right"|36
|
|BELIEF_MESSIAH
|-
|align="right"|37
|
|BELIEF_MISSIONARY_ZEAL
|-
|align="right"|38
|
|BELIEF_HOLY_ORDER
|-
|align="right"|39
|
|BELIEF_RELIGIOUS_UNITY
|-
|align="right"|40
|
|BELIEF_CATHEDRALS
|-
|align="right"|41
|
|BELIEF_MOSQUES
|-
|align="right"|42
|
|BELIEF_PAGODAS
|-
|align="right"|43
|
|BELIEF_MONASTERIES
|-
|align="right"|44
|
|BELIEF_PEACE_GARDENS
|-
|align="right"|45
|
|BELIEF_CHORAL_MUSIC
|-
|align="right"|46
|
|BELIEF_RELIGIOUS_ART
|-
|align="right"|47
|
|BELIEF_LITURGICAL_DRAMA
|-
|align="right"|48
|
|BELIEF_ASCETISM
|-
|align="right"|49
|
|BELIEF_RELIGIOUS_CENTER
|-
|align="right"|50
|
|BELIEF_PAPAL_PRIMACY
|-
|align="right"|51
|
|BELIEF_DANCE_AURORA
|-
|align="right"|52
|
|BELIEF_RELIGIOUS_COMMUNITY
|-
|align="right"|53
|
|BELIEF_DIVINE_INSPIRATION
|-
|align="right"|54
|
|BELIEF_PILGRIMAGE
|-
|align="right"|55
|
|BELIEF_WORLD_CHURCH
|}</code>


= Examples =
Here is how to use the LUA enumeration to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value -1.
<syntaxhighlight lang="lua" class="civ5-example">
local id = BeliefTypes.NO_BELIEF
local id = BeliefTypes["NO_BELIEF"]
</syntaxhighlight>
Here are different ways to query the database to retrieve the ''ID'' from the ''type''. Those examples will return and assign the integer value 0. See also {{Type5|GameInfo}}.
<syntaxhighlight lang="lua" class="civ5-example">
local id = GameInfo.Beliefs.BELIEF_GODDESS_HUNT.ID
local id = GameInfo["Beliefs"].["BELIEF_GODDESS_HUNT"].ID
local id = GameInfo.Beliefs{Type="BELIEF_GODDESS_HUNT"}().ID
</syntaxhighlight>
Alternatively you could use the ''ID'' or the ''type'' to retrieve the value of the ''Description'' column. Those examples will return and assign the value TXT_KEY_BELIEF_GODDESS_HUNT.
<syntaxhighlight lang="lua" class="civ5-example">
local description = GameInfo.Beliefs[0].Description
local description = GameInfo["Beliefs"][0]["Description"]
local description = GameInfo.Beliefs{ID=0}().Description
</syntaxhighlight>


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
ENHANCERELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|EnhanceReligion}}<b>(</b>{{Type5|PlayerID}} vaticanPlayer, {{Type5|ReligionType}} religion, {{Type5|BeliefType}} belief4, {{Type5|BeliefType}} belief5<b>)</b></code>
<!-- 
FOUNDPANTHEON
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|FoundPantheon}}<b>(</b>'''int''' vaticanPlayer, {{Type5|BeliefType}} belief1<b>)</b></code>
<!-- 
FOUNDRELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|FoundReligion}}<b>(</b>{{Type5|PlayerID}} vaticanPlayer, {{Type5|ReligionType}} religion, '''unknown''' arg2, {{Type5|BeliefType}} belief2, {{Type5|BeliefType}} belief3, {{Type5|BeliefType}} belief3, '''int''' arg6, {{Type5|City}} vaticanCity<b>)</b></code>
<!-- 
GETAVAILABLEBONUSBELIEFS
-->
|-
|align="right" width="200" |<code>iterator('''int''', {{Type5|BeliefType}})</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetAvailableBonusBeliefs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAVAILABLEENHANCERBELIEFS
-->
|-
|align="right" width="200" |<code>iterator('''int''', {{Type5|BeliefType}})</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetAvailableEnhancerBeliefs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAVAILABLEFOLLOWERBELIEFS
-->
|-
|align="right" width="200" |<code>iterator('''int''', {{Type5|BeliefType}})</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetAvailableFollowerBeliefs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAVAILABLEFOUNDERBELIEFS
-->
|-
|align="right" width="200" |<code>iterator('''int''', {{Type5|BeliefType}})</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetAvailableFounderBeliefs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETAVAILABLEPANTHEONBELIEFS
-->
|-
|align="right" width="200" |<code>iterator('''int''', {{Type5|BeliefType}})</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetAvailablePantheonBeliefs}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBELIEFSINRELIGION
-->
|-
|align="right" width="200" |<code>iterator('''int''', {{Type5|BeliefType}})</code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|GetBeliefsInReligion}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SENDFOUNDPANTHEON
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendFoundPantheon}}<b>(</b>{{Type5|PlayerID}} arg0, {{Type5|BeliefType}} Belief<b>)</b></code>
<!-- 
SENDFOUNDRELIGION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Network}}.{{Func5|Network|SendFoundReligion}}<b>(</b>{{Type5|PlayerID}} arg0, {{Type5|ReligionType}} CurrentReligion, '''unknown''' customName, '''unknown''' arg3, '''unknown''' arg4, {{Type5|BeliefType}} arg5, {{Type5|BeliefType}} arg6, '''int''' cityX, '''int''' cityY<b>)</b></code>
<!-- 
GETBELIEFINPANTHEON
-->
|-
|align="right" width="200" |<code>{{Type5|BeliefType}}</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetBeliefInPantheon}}<b>(</b><!-- No arguments --><b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|BeliefType]]