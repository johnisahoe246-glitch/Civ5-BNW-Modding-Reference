The '''GlobalTypes.xml''' file defines many of the XML names referenced in other files.  Changes to many of these entries must be reflected by [[CvEnums|CvEnums.h]] in the SDK.

All tags must be opened and closed; the first is the "open", the second the "close" tag. If nothing goes inside a "list tag", then it should just be the opening tag with a "/" before the closing bracket. The following tables contain all available tags, as well as their purpose and accepted values. 

<font color=red>This page is missing information.
Do not remove this notice until it is complete.</font>


==Tags==
===Lists (Multi-line)===

All List tags consist of an opening/closing tag, which is shown here, and then each entry within it is another tag with the same name as the parent tag, minus the "s" (i.e. singular, rather than plural).

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!AnimationOperatorTypes
|Unknown
 <AnimationOperatorTypes>
  <!--Changes must be reflected in CvEnums.h-->
  <AnimationOperatorType>RAND_FPR</AnimationOperatorType>
  <AnimationOperatorType>SET_FPR</AnimationOperatorType>
  <AnimationOperatorType>SET_BR</AnimationOperatorType>
 </AnimationOperatorTypes>
|-
!FinctionTypes
|Unknown
 <FunctionTypes>
  <!--Changes must be reflected in CvEnums.h-->
  <FunctionType>FUNC_NOINTERP</FunctionType>
  <FunctionType>FUNC_LINKEY</FunctionType>
  <FunctionType>FUNC_BEZKEY</FunctionType>
  <FunctionType>FUNC_TCBKEY</FunctionType>
  <FunctionType>FUNC_EULERKEY</FunctionType>
 </FunctionTypes>
|-
!FlavorTypes
|The different flavors availalbe for AI personalities
 <FlavorTypes>
  <FlavorType>FLAVOR_MILITARY</FlavorType>
  <FlavorType>FLAVOR_RELIGION</FlavorType>
  <FlavorType>FLAVOR_PRODUCTION</FlavorType>
 </FlavorTypes>
|-
!ArtStyleTypes
|Art styles for cities
 <ArtStyleTypes>
  <ArtStyleType>ARTSTYLE_EUROPEAN</ArtStyleType>
  <ArtStyleType>ARTSTYLE_ASIAN</ArtStyleType>
  <ArtStyleType>ARTSTYLE_SOUTH_AMERICA</ArtStyleType>
 </ArtStyleTypes>
|-
!CitySizeTypes
|Types of city sizes
 <CitySizeTypes>
  <CitySizeType>CITYSIZE_SMALL</CitySizeType>
  <CitySizeType>CITYSIZE_MEDIUM</CitySizeType>
  <CitySizeType>CITYSIZE_LARGE</CitySizeType>
 </CitySizeTypes>
|-
!ContactTypes
|Different reasons AI civs may contact other civs
 <ContactTypes>
  <!--Changes must be reflected in CvEnums.h-->
  <ContactType>CONTACT_RELIGION_PRESSURE</ContactType>
  <ContactType>CONTACT_CIVIC_PRESSURE</ContactType>
  <ContactType>CONTACT_JOIN_WAR</ContactType>
 </ContactTypes>
|-
!DiplomacyPowerTypes
|Different power relations between civs available for diplomacy
 <DiplomacyPowerTypes>
  <!--Changes must be reflected in CvEnums.h-->
  <DiplomacyPowerType>DIPLOMACYPOWER_WEAKER</DiplomacyPowerType>
  <DiplomacyPowerType>DIPLOMACYPOWER_EQUAL</DiplomacyPowerType>
  <DiplomacyPowerType>DIPLOMACYPOWER_STRONGER</DiplomacyPowerType>
 </DiplomacyPowerTypes>
|-
!AutomateTypes
|Different ways a human can automate things
 <AutomateTypes>
  <!--Changes must be reflected in CvEnums.h-->
  <AutomateType>AUTOMATE_BUILD</AutomateType>
  <AutomateType>AUTOMATE_NETWORK</AutomateType>
  <AutomateType>AUTOMATE_CITY</AutomateType>
  <AutomateType>AUTOMATE_EXPLORE</AutomateType>
  <AutomateType>AUTOMATE_RELIGION</AutomateType>
 </AutomateTypes>
|-
!DirectionTypes
|The direction a unit can look into at the map; used e.g. in the unit spawning command and excessively used in Afterworld
 <DirectionTypes>
  <!--Changes must be reflected in CvEnums.h-->
  <DirectionType>DIRECTION_NORTH</DirectionType>
  <DirectionType>DIRECTION_NORTHEAST</DirectionType>
  <DirectionType>DIRECTION_EAST</DirectionType>
 </DirectionTypes>
|-
!FootstepAudioTypes
|Different sound types for unit movement
 <FootstepAudioTypes>
  <FootstepAudioType>FOOTSTEP_AUDIO_HUMAN</FootstepAudioType>
  <FootstepAudioType>FOOTSTEP_AUDIO_HUMAN_LOW</FootstepAudioType>
  <FootstepAudioType>FOOTSTEP_AUDIO_ANIMAL</FootstepAudioType>
 </FootstepAudioTypes>
|-
!FootstepAudioTags
|Associtaes the FootstepAudioTypes with audio files
 <FootstepAudioTags>
  <FootstepAudioTag>
   <FootstepAudioType>FOOTSTEP_AUDIO_HUMAN</FootstepAudioType>
   <FootstepAudioTagString>AS3D_UN_FOOT_UNIT</FootstepAudioTagString>
  </FootstepAudioTag>
  <FootstepAudioTag>
   <FootstepAudioType>FOOTSTEP_AUDIO_HUMAN_LOW</FootstepAudioType>
   <FootstepAudioTagString>AS3D_UN_FOOT_UNIT_LOW</FootstepAudioTagString>
  </FootstepAudioTag>
 </FootstepAudioTags>
|-
!InterfaceVisibilityTypes
|Status, which the interface can have. E.g. the interface is hidden while you look at the different advisors
 <InterfaceVisibilityTypes>
  <InterfaceVisibilityType>INTERFACE_SHOW</InterfaceVisibilityType>
  <InterfaceVisibilityType>INTERFACE_HIDE</InterfaceVisibilityType>
  <InterfaceVisibilityType>INTERFACE_HIDE_ALL</InterfaceVisibilityType>
 </InterfaceVisibilityTypes>
|}

{{Civ4_XML_Files}}