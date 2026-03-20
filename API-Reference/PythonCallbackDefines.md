The '''PythonCallbackDefines.xml''' file was added in the Beyond the Sword expansion to disable some unnecessary callbacks. A callback is a python function called from the SDK, and some callbacks were called often but did not actually do anything. This file allows you to disable or enable the callbacks listed in it.

All tags must be opened and closed; the first is the "open", the second the "close" tag. If nothing goes inside a "list tag", then it should just be the opening tag with a "/" before the closing bracket. The following tables contain all available tags, as well as their purpose and accepted values. 

==Tags==
===Headers===

These tags typically bracket other tags, sometimes the entire file, and are generally used to specify more than one piece of data.

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!Civ4Defines
|Begins and ends the file. Everything must go between these two tags
|-
!Define
|Begins and ends an individual python callback define
|}


===Text===

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!DefineName
|The python callback that is being defined in each entry
|}


===Integers===

All of these tags have a numerical value.  Though it sometimes can be negative, it usually is not.

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!iDefineIntValue
|Defines whether the game will use the callback, acts like a boolean
|}


==Callbacks Disabled==

All of the callbacks listed below are disabled in Beyond the Sword

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Calllback Name
! style="background:#efefef;" | Python File
|-
!cannotFoundCity
|[[CvGameUtils]]
|-
!canFoundCitiesOnWater
|CvGameUtils
|-
!isPlayerResearch
|CvGameUtils
|-
!canResearch
|CvGameUtils
|-
!cannotDoCivic
|CvGameUtils
|-
!canDoCivic
|CvGameUtils
|-
!cannotConstruct
|CvGameUtils
|-
!canConstruct
|CvGameUtils
|-
!canDeclareWar
|CvGameUtils
|-
!cannotResearch
|CvGameUtils
|-
!getUnitCostMod
|CvGameUtils
|-
!getBuildingCostMod
|CvGameUtils
|-
!getCityFoundValue
|CvGameUtils
|-
!getBuildingCostMod
|CvGameUtils
|-
!cannotHandleAction
|CvGameUtils
|-
!canBuild
|CvGameUtils
|-
!cannotTrain
|CvGameUtils
|-
!canTrain
|CvGameUtils
|-
!unitCannotMoveInto
|CvGameUtils
|-
!getBuildingCostMod
|CvGameUtils
|-
!cannotSpreadReligion
|CvGameUtils
|-
!finishText
|Unknown
|-
!onUnitSetXY
|[[CvEventManager]]
|-
!onUnitSelected
|CvEventManager
|-
!onUnitSelected
|CvEventManager
|-
!onUpdate
|CvEventManager
|-
!onUnitCreated
|CvEventManager
|-
!onUnitLost
|CvEventManager
|}


==Example==

  <Define>
   <DefineName>USE_CAN_TRAIN_CALLBACK</DefineName>
   <iDefineIntVal>0</iDefineIntVal>
  </Define>

{{Civ4_XML_Files}}