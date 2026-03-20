{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|ID.png|The <code>PolicyType</code> pseudo-type is actually a regular '''integer'''. Pseudo-types do not exist in Lua, they only serve a documentation purpose on the wiki!
* {{DB}} Integers labeled as <code>PolicyType</code> corresponds to the ''ID'' column of the {{Table5|Policies|CIV5Policies}} XML table.
}}


= XML: the Policies table =
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
|POLICY_LIBERTY
|-
|align="right"|1
|
|POLICY_COLLECTIVE_RULE
|-
|align="right"|2
|
|POLICY_CITIZENSHIP
|-
|align="right"|3
|
|POLICY_REPUBLIC
|-
|align="right"|4
|
|POLICY_REPRESENTATION
|-
|align="right"|5
|
|POLICY_MERITOCRACY
|-
|align="right"|6
|
|POLICY_TRADITION
|-
|align="right"|7
|
|POLICY_ARISTOCRACY
|-
|align="right"|8
|
|POLICY_OLIGARCHY
|-
|align="right"|9
|
|POLICY_LEGALISM
|-
|align="right"|10
|
|POLICY_LANDED_ELITE
|-
|align="right"|11
|
|POLICY_MONARCHY
|-
|align="right"|12
|
|POLICY_HONOR
|-
|align="right"|13
|
|POLICY_WARRIOR_CODE
|-
|align="right"|14
|
|POLICY_DISCIPLINE
|-
|align="right"|15
|
|POLICY_MILITARY_TRADITION
|-
|align="right"|16
|
|POLICY_MILITARY_CASTE
|-
|align="right"|17
|
|POLICY_PROFESSIONAL_ARMY
|-
|align="right"|18
|
|POLICY_PIETY
|-
|align="right"|19
|
|POLICY_ORGANIZED_RELIGION
|-
|align="right"|20
|
|POLICY_MANDATE_OF_HEAVEN
|-
|align="right"|21
|
|POLICY_THEOCRACY
|-
|align="right"|22
|
|POLICY_REFORMATION
|-
|align="right"|23
|
|POLICY_FREE_RELIGION
|-
|align="right"|24
|
|POLICY_PATRONAGE
|-
|align="right"|25
|
|POLICY_PHILANTHROPY
|-
|align="right"|26
|
|POLICY_AESTHETICS
|-
|align="right"|27
|
|POLICY_SCHOLASTICISM
|-
|align="right"|28
|
|POLICY_CULTURAL_DIPLOMACY
|-
|align="right"|29
|
|POLICY_EDUCATED_ELITE
|-
|align="right"|30
|
|POLICY_COMMERCE
|-
|align="right"|31
|
|POLICY_TRADE_UNIONS
|-
|align="right"|32
|
|POLICY_NAVAL_TRADITION
|-
|align="right"|33
|
|POLICY_MERCANTILISM
|-
|align="right"|34
|
|POLICY_MERCHANT_NAVY
|-
|align="right"|35
|
|POLICY_PROTECTIONISM
|-
|align="right"|36
|
|POLICY_RATIONALISM
|-
|align="right"|37
|
|POLICY_SECULARISM
|-
|align="right"|38
|
|POLICY_HUMANISM
|-
|align="right"|39
|
|POLICY_FREE_THOUGHT
|-
|align="right"|40
|
|POLICY_SOVEREIGNTY
|-
|align="right"|41
|
|POLICY_SCIENTIFIC_REVOLUTION
|-
|align="right"|42
|
|POLICY_FREEDOM
|-
|align="right"|43
|
|POLICY_CONSTITUTION
|-
|align="right"|44
|
|POLICY_UNIVERSAL_SUFFRAGE
|-
|align="right"|45
|
|POLICY_CIVIL_SOCIETY
|-
|align="right"|46
|
|POLICY_FREE_SPEECH
|-
|align="right"|47
|
|POLICY_DEMOCRACY
|-
|align="right"|48
|
|POLICY_ORDER
|-
|align="right"|49
|
|POLICY_UNITED_FRONT
|-
|align="right"|50
|
|POLICY_SOCIALISM
|-
|align="right"|51
|
|POLICY_NATIONALISM
|-
|align="right"|52
|
|POLICY_PLANNED_ECONOMY
|-
|align="right"|53
|
|POLICY_COMMUNISM
|-
|align="right"|54
|
|POLICY_AUTOCRACY
|-
|align="right"|55
|
|POLICY_POPULISM
|-
|align="right"|56
|
|POLICY_MILITARISM
|-
|align="right"|57
|
|POLICY_FASCISM
|-
|align="right"|58
|
|POLICY_POLICE_STATE
|-
|align="right"|59
|
|POLICY_TOTAL_WAR
|-
|align="right"|60
|
|POLICY_TRADITION_FINISHER
|-
|align="right"|61
|
|POLICY_LIBERTY_FINISHER
|-
|align="right"|62
|
|POLICY_HONOR_FINISHER
|-
|align="right"|63
|
|POLICY_PIETY_FINISHER
|-
|align="right"|64
|
|POLICY_PATRONAGE_FINISHER
|-
|align="right"|65
|
|POLICY_COMMERCE_FINISHER
|-
|align="right"|66
|
|POLICY_RATIONALISM_FINISHER
|-
|align="right"|67
|
|POLICY_FREEDOM_FINISHER
|-
|align="right"|68
|
|POLICY_ORDER_FINISHER
|-
|align="right"|69
|
|POLICY_AUTOCRACY_FINISHER
|}</code>


= Examples =


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
HANDLEACTION
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Game}}.{{Func5|Game|HandleAction}}<b>(</b>{{Type5|PolicyType}} action<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|GridButton}}:{{Func5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} arg0, ('''void''' func<b>(</b>{{Type5|PolicyType}} Id, {{Type5|ResourceType}} none, {{Type5|Button}} control<b>)</b>) OnEndTurnClicked<b>)</b></code>
<!-- 
CANADOPTPOLICY
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|CanAdoptPolicy}}<b>(</b>{{Type5|PolicyType}} policy<b>)</b></code>
<!-- 
DOADOPTPOLICY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|DoAdoptPolicy}}<b>(</b>{{Type5|PolicyType}} policy<b>)</b></code>
<!-- 
GETPOLICYBRANCHCHOSEN
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|GetPolicyBranchChosen}}<b>(</b>{{Type5|PolicyType}} policyBranch<b>)</b></code>
<!-- 
HASPOLICY
-->
|-
|align="right" width="200" |<code>'''int'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|HasPolicy}}<b>(</b>{{Type5|PolicyType}} policy<b>)</b></code>
<!-- 
ISPOLICYBLOCKED
-->
|-
|align="right" width="200" |<code>'''bool'''</code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|IsPolicyBlocked}}<b>(</b>{{Type5|PolicyType}} i<b>)</b></code>
<!-- 
SETHASPOLICY
-->
|-
|align="right" width="200" |<code><!-- No return type --></code>
|style="padding-left:6px" |<code>{{Type5|Player}}:{{Func5|Player|SetHasPolicy}}<b>(</b>{{Type5|PolicyType}} index, '''bool''' newValue<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|PolicyType]]