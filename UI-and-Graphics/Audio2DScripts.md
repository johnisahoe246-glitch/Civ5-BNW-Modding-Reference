The '''Audio2DScripts''' file defines the primary background and foreground sounds for each screen and playing attribute. These include the music for the opening, map and diplomacy screens and the primary background for the city screen. Foreground sounds include those for tech discoveries, structure and unit builds, and mouse clicks.

All tags must be opened and closed; the first is the "open", the second the "close" tag. If nothing goes inside a "list tag", then it should just be the opening tag with a "/" before the closing bracket. The following tables contain all available tags, as well as their purpose and accepted values. 

<font color=red>This page is missing information.
Do not remove this notice until it is complete.</font>


==Tags==
===Text===
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!ScriptID
| This is the name of the sound object used by the Audio2D script. This ID is used in [[CIV4LeaderHeadInfos]], [[AudioSoundscapeScripts]] and by Python CyAudioGame.Play2DSound() function. The IDs are prefixed with AS2D_ for easier identification and followed by the filename.
|-
!SoundID
| Implemented in AudioDefines to retrieve the sound file.
|-
!SoundType
| Indicates which volume slider to use under Game Options -> Audio AMBIENCE, INTERFACE, MUSIC, SFX or SPEECH.  These are prefixed with GAME_ for easy identification. Values are defined in AudioDefines.
|}


===Integer===

All of these tags have a numerical value.  Though it sometimes can be negative, it usually is not.

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!iMinVolume
| Minimum volume to play this sound. Values are from 0 to 100.
|-
!iMaxVolume
| Maximum volume to play this sound. Values are from 0 to 100.
|-
!iPitchChangeDown
| <font color=red>unknown.</font> Set to 0.
|-
!iPitchChangeUp
| <font color=red>unknown.</font> Set to 0.
|-
!iMinLeftPan
| <font color=red>unknown.</font> Set to -1.
|-
!iMaxLeftPan
| <font color=red>unknown.</font> Set to -1.
|-
!iMinRightPan
| <font color=red>unknown.</font> Set to -1.
|-
!iMaxRightPan
| <font color=red>unknown.</font> Set to -1.
|-
!iMinTimeDelay
| <font color=red>unknown.</font> Minimum time in delay playing sound. Values in milliseconds.
|-
!iMaxTimeDelay
| <font color=red>unknown.</font> Maximum time in delay playing sound. Values in milliseconds.
|-
!iLengthOfSound
| <font color=red>unknown.</font> Set to 0.
|-
!iNotPlayPercent
| <font color=red>unknown.</font> Set to 0.  (Beyond the Sword only)
|}


===Boolean===

All of these can either be 1 (on, or true) or 0 (off, or false).  Be careful, as you can wind up with a double-negative, which the game will interpret as "True".

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!bLooping
| Indicates whether the sound will "loop" (repeat indefinitely).
|-
!bTaperForSoundtracks
| <font color=red>unknown.</font> Set to 0.
|}


===Floating-Point===
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!fMinDryLevel
| <font color=red>unknown.</font> Set to 1.0.
|-
!fMaxDryLevel
| <font color=red>unknown.</font> Set to 1.0.
|-
!fMinWetLevel
| <font color=red>unknown.</font> Set to 0.0.
|-
!fMaxWetLevel
| <font color=red>unknown.</font> Set to 0.0.
|}


==Example==

In the following example of code, please note that there is a specific order of all of the tags.  You ''must'' list the tags in this order for the game to properly interpret your file.

 <Script2DSound>
    <ScriptID>AS2D_ERROR</ScriptID>
    <SoundID>SND_ERROR</SoundID>
    <SoundType>GAME_SFX</SoundType>
    <iMinVolume>80</iMinVolume>
    <iMaxVolume>80</iMaxVolume>
    <iPitchChangeDown>0</iPitchChangeDown>
    <iPitchChangeUp>0</iPitchChangeUp>
    <iMinLeftPan>-1</iMinLeftPan>
    <iMaxLeftPan>-1</iMaxLeftPan>
    <iMinRightPan>-1</iMinRightPan>
    <iMaxRightPan>-1</iMaxRightPan>
    <bLooping>0</bLooping>
    <iMinTimeDelay>0</iMinTimeDelay>
    <iMaxTimeDelay>0</iMaxTimeDelay>
    <bTaperForSoundtracks>0</bTaperForSoundtracks>
    <iLengthOfSound>0</iLengthOfSound>
    <fMinDryLevel>1.0</fMinDryLevel>
    <fMaxDryLevel>1.0</fMaxDryLevel>
    <fMinWetLevel>0.0</fMinWetLevel>
    <fMaxWetLevel>0.0</fMaxWetLevel>
 </Script2DSound>

{{Civ4_XML_Files}}