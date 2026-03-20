The '''AudioSoundscapeScripts''' file groups the 2D and 3D sounds together to form "soundscapes" which are used in various parts of the game.

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
| The name of the audio soundscape script prefixed with ASSS_ for easier identification.
|}


===Integer===

All of these tags have a numerical value.  Though it sometimes can be negative, it usually is not.

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!iMinVolume
| Minimum volume for all sounds in this soundscape.
|-
!iMaxVolume
| Maximum volume for all sounds in this soundscape.
|}


===Lists (Multi-line)===

All List tags consist of an opening/closing tag, which is shown here, and then each entry within it is another tag with the same name as the parent tag, minus the "s" (i.e. singular, rather than plural).

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!SoundscapeElement
| The audio script object and the script engine it uses. Generally this will consist of one primary screen background using the 2D script engine and multiple additional sounds using the 3D script engine.
|-
!ScriptType
| The audio script engine. Defined in [[AudioDefines]]. Values are 2D or 3D.
|-
!ScriptID
| The sound name defined in Audio2DScripts or Audio3DScripts.
|}


==Example==

In the following example of code, please note that there is a specific order of all of the tags.  You ''must'' list the tags in this order for the game to properly interpret your file.

 <ScriptSoundscape>
    <ScriptID>ASSS_CITY_LATE_LARGE_SELECT_AMB</ScriptID>
    <iMinVolume>100</iMinVolume>
    <iMaxVolume>100</iMaxVolume>
    <SoundscapeElement>
        <ScriptType>2D</ScriptType>
        <ScriptID>AS2D_SS_CITY_LATE_LARGE_BED</ScriptID>
    </SoundscapeElement>
    <SoundscapeElement>
        <ScriptType>3D</ScriptType>
        <ScriptID>AS3D_SS_HORN</ScriptID>
    </SoundscapeElement>
    <SoundscapeElement>
        <ScriptType>3D</ScriptType>
        <ScriptID>AS3D_SS_AUTO_PASSING</ScriptID>
    </SoundscapeElement>
    <SoundscapeElement>
        <ScriptType>3D</ScriptType>
        <ScriptID>AS3D_SS_FOOTSTEPS</ScriptID>
    </SoundscapeElement>
    <SoundscapeElement>
        <ScriptType>3D</ScriptType>
        <ScriptID>AS3D_SS_HORN_DOPPLER</ScriptID>
    </SoundscapeElement>
    <SoundscapeElement>
        <ScriptType>3D</ScriptType>
        <ScriptID>AS3D_SS_SIREN</ScriptID>
    </SoundscapeElement>
 </ScriptSoundscape>

{{Civ4_XML_Files}}