The '''Audio3DScripts''' file defines attributes for sounds used by 3D sound script operations. These attributes define how and if sound is played at a distance from a source. Most notably, when you are zoomed into a resource (e.g. cows) on the map screen, they are louder the closer you are zoomed in and if they are centered on the screen.

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
| The script object name prefixed with AS3D_ followed by the file name. Used in [[AudioSoundscapeScripts]] and by Python CyAudioGame.Play3DSound() function.
|-
!SoundID
| Implemented in [[AudioDefines]] to retrieve the sound file.
|-
!SoundType
| Indicates which volume slider to use under Game Option -> Audio. Values are defined in [[AudioDefines]] and are prefixed with GAME_. Values are AMBIENCE, INTERFACE, MUSIC, SFX or SPEECH.
|-
!StartPosition
| Position to player where the sounds appears to come from when it starts (most effective for surround sound setups.) Values are defined in [[AudioDefines]]. Values are NONE, RANDOM, ALL, FRONT, BACK, BACK_LEFT, BACK_RIGHT, LEFT, RIGHT, FRONT_LEFT, FRONT_RIGHT and REARS
|-
!EndPosition
| Position to player where the sounds appears to come from when it ends (most effective for surround sound setups.) Values are defined in [[AudioDefines]]. Values are NONE, RANDOM, ALL, FRONT, BACK, BACK_LEFT, BACK_RIGHT, LEFT, RIGHT, FRONT_LEFT, FRONT_RIGHT and REARS
|}


===Integer===

All of these tags have a numerical value.  Though it sometimes can be negative, it usually is not.

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!iMinVolume
| Minimum volume to play this sound. Values from 0 to 100.
|-
!iMaxVolume
| Maximum volume to play this sound. Values from 0 to 100.
|-
!iPitchChangeDown
| <font color=red>unknown.</font> Negative values (in Hz? Known values are 0, -2000, -3000, -4000, -5000, -7000)
|-
!iPitchChangeUp
| <font color=red>unknown.</font> Positive values (in Hz? known values are 0, 2000, 3000, 4000, 5000, 7000)
|-
!iMinTimeDelay
| <font color=red>unknown.</font> Minimum time delay before playing sound. Values in milliseconds
|-
!iMaxTimeDelay
| <font color=red>unknown.</font> Maximum time delay before playing sound. Values in milliseconds.
|-
!iLengthOfSound
| <font color=red>unknown.</font> Set to 0.
|-
!iMinVelocity
| <font color=red>unknown.</font> Minimum velocity to play the sound. Set to 0
|-
!iMaxVelocity
| <font color=red>unknown.</font> Maximum velocity to play the sound. Set to 0.
|-
!iMinDistanceFromListener
| <font color=red>unknown.</font> Minimum distance in meters from listen before playing the sound.
|-
!iMaxDistanceFromListener
| <font color=red>unknown.</font> Maximum distance in meters from listen before playing the sound.
|-
!iMinDistanceForMaxVolume
| Minimum distance in meters to play the sound at maximum volume.
|-
!iMaxDistanceForMaxVolume
| Maximum distance in meters to play the sound at maximum volume.
|-
!iMinCutoffDistance
| Minimum distance in meters before stop playing the sound.
|-
!iMaxCutoffDistance
| Maximum distance in meters before stop playing the sound.
|-
!iNotPlayPercent
| <font color=red>unknown.</font> Set to 0. (Beyond the Sword only)
|}


===Boolean===

All of these can either be 1 (on, or true) or 0 (off, or false).  Be careful, as you can wind up with a double-negative, which the game will interpret as "True".

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!bLooping
| Indicates whether the sound will "loop", ie: repeat indefinitely.
|-
!bTaperForSoundtracks
| <font color=red>unknown.</font> Set to 0.
|}


===Floating===
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
| <font color=red>unknown.</font> Values between 0.0 - 1.0.
|-
!fMaxWetLevel
| <font color=red>unknown.</font> Values between 0.0 - 1.0.
|}


==Example==

In the following example of code, please note that there is a specific order of all of the tags.  You ''must'' list the tags in this order for the game to properly interpret your file.

 <Script3DSound>
    <ScriptID>AS3D_ERROR</ScriptID>
    <SoundID>SND_ERROR</SoundID>
    <SoundType>GAME_SFX</SoundType>
    <iMinVolume>80</iMinVolume>
    <iMaxVolume>80</iMaxVolume>
    <iPitchChangeDown>0</iPitchChangeDown>
    <iPitchChangeUp>0</iPitchChangeUp>
    <bLooping>0</bLooping>
    <iMinTimeDelay>0</iMinTimeDelay>
    <iMaxTimeDelay>0</iMaxTimeDelay>
    <StartPosition>FRONT</StartPosition>
    <EndPosition>FRONT</EndPosition>
    <iMinVelocity>0</iMinVelocity>
    <iMaxVelocity>0</iMaxVelocity>
    <iMinDistanceFromListener>0</iMinDistanceFromListener>
    <iMaxDistanceFromListener>0</iMaxDistanceFromListener>
    <iMinDistanceForMaxVolume>100000</iMinDistanceForMaxVolume>
    <iMaxDistanceForMaxVolume>100000</iMaxDistanceForMaxVolume>
    <iMinCutoffDistance>100000</iMinCutoffDistance>
    <iMaxCutoffDistance>100000</iMaxCutoffDistance>
    <bTaperForSoundtracks>0</bTaperForSoundtracks>
    <iLengthOfSound>0</iLengthOfSound>
    <fMinDryLevel>1.0</fMinDryLevel>
    <fMaxDryLevel>1.0</fMaxDryLevel>
    <fMinWetLevel>0.0</fMinWetLevel>
    <fMaxWetLevel>0.0</fMaxWetLevel>
 </Script3DSound>

{{Civ4_XML_Files}}