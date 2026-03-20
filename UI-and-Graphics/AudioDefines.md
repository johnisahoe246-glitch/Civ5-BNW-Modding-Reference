The '''AudioDefines''' file contains SoundIDs for sounds used in-game. [[Audio2DScripts]] and [[Audio3DScripts]], among other files, refer to the SoundIDs listed here.

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
!SoundID
| The name of the Sound ID that other files reference. Prefixed with identifiers such as SND_, SONG_, or DIPLO_ for easier identification.
|-
!Filename
| The location of the sound file (or files) that contain the audio data for the sound. These are .wav files for sound effects, and .mp3 files for the soundtrack and diplomacy music.
Note that the file extension (.wav or .mp3) should '''not''' be included here; only include the filename (e.g. Sounds/Error.wav is listed as Sounds/Error). Furthermore, collections of sounds (usually for unit responses) such as BabylonOrder-000.wav, BabylonOrder-001.wav, BabylonOrder-002.wav, etc. are '''collectively''' referenced simply as 'BabylonOrder'. When the sound with this SoundID is played in-game, the sounds makred -000, -001, -002, etc. are selected such that they are different each time. This ensures that if you click on a unit, it will not say the same thing over and over again, and will instead have a variety of differing responses.
|-
!LoadType
| How the sound should be loaded. Types are: RESIDENT -- sound is loaded with the game on startup; STREAMED -- sound is streamed from the disk, not requiring the completion of loading before the sound begins to play (used for larger file sizes such as music or lengthy ambiances); DYNAMIC_RES -- sound is loaded as needed from the disk and played upon completion of loading (used for virtually all sound effects and other small file sizes).
|}


===Boolean===

All of these can either be 1 (on, or true) or 0 (off, or false).  Be careful, as you can wind up with a double-negative, which the game will interpret as "True".

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!bIsCompressed
| <font color=red>Unknown.</font> Always 1. (Could theoretically be set to 0 if the sound is not compressed, although the effects of doing so are unknown.)
|-
!bInGeneric
| <font color=red>Unknown.</font> Always 1.
|}



==Example==

In the following example of code, please note that there is a specific order of all of the tags.  You ''must'' list the tags in this order for the game to properly interpret your file.

 <SoundData>
 	<SoundID>SND_MONGOL_ORDER</SoundID>
 	<Filename>Sounds/Units/MongolOrder</Filename>
 	<LoadType>DYNAMIC_RES</LoadType>
 	<bIsCompressed>1</bIsCompressed>
 	<bInGeneric>1</bInGeneric>
 </SoundData>


==Other Data==
This data appears after the entries for the sound files.

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!ContextTypes
|Unknown
 <ContextTypes>
  <ContextType>Generic</ContextType>
 </ContextTypes>
|-
!SoundTypes
|Types of sounds that can appear in game
 <SoundTypes>
  <SoundType>GAME_MUSIC</SoundType>
  <SoundType>GAME_SFX</SoundType>
  <SoundType>GAME_SPEECH</SoundType>
  <SoundType>GAME_AMBIENCE</SoundType>
  <SoundType>GAME_INTERFACE</SoundType>
 </SoundTypes>
|-
!PositionTypes
|Unknown
 <PositionTypes>
  <PositionType>NONE</PositionType>
  <PositionType>FRONT</PositionType>
  <PositionType>BACK</PositionType>
 </PositionTypes>
|-
!ScriptTypes
|Types of audio scripts
 <ScriptTypes>
  <ScriptType>NONE</ScriptType>
  <ScriptType>2D</ScriptType>
  <ScriptType>3D</ScriptType>
  <ScriptType>SOUNDSCAPE</ScriptType>
 </ScriptTypes>
|-
!LoadTypes
|Unknown
 <LoadTypes>
  <LoadType>RESIDENT</LoadType>
  <LoadType>DYNAMIC_RES</LoadType>
  <LoadType>STREAMED</LoadType>
 </LoadTypes>
|-
!EffectTypes
|Unknown
 <EffectTypes>
  <EffectType>GENERIC</EffectType>
  <EffectType>PADDEDCELL</EffectType>
  <EffectType>ROOM</EffectType>
 </EffectTypes>
|-
!GameEnvironmentTypes
|Unknown
 <GameEnvironmentTypes>
  <GameEnvironmentType>GENERAL</GameEnvironmentType>
 </GameEnvironmentTypes>
|-
!Effects
|Unknown
 <Effects>
  <GameEnvironmentMap>
   <GameEnvironmentType>GENERAL</GameEnvironmentType>
   <ReverbData>
    <fReverbTime>1.0</fReverbTime>
    <fReverbPredelay>0.0</fReverbPredelay>
    <fReverbDamping>0.0</fReverbDamping>
    <fReverbDryLevel>1.0</fReverbDryLevel>
    <fReverbWetLevel>0.0</fReverbWetLevel>
   </ReverbData>
   <EffectType>FOREST</EffectType>
  </GameEnvironmentMap>
 </Effects>
|-
!GameEnvironmentMap
|Unknown; nested in Effects
|-
!GameEnvironmentType
|Unknown; nseted in GameEnvironmentMap
|-
!ReverbData
|Unknown; nested in GameEnvironmentMap
|-
!EffectType
|Unknown; nested in GameEnvironmentMap
|-
!SpeakerConfigs
|Unknown
 <SpeakerConfigs>
  <SpeakerConfig>TXT_KEY_OPTION_SOUND_STEREO</SpeakerConfig>
  <SpeakerConfig>TXT_KEY_OPTION_SOUND_HEADPHONES</SpeakerConfig>
  <SpeakerConfig>Dolby Surround</SpeakerConfig>
  <SpeakerConfig>SRS Circle Surround</SpeakerConfig>
 </SpeakerConfigs>
|-
!AudioSystemInit
|Unknown
 <AudioSystemInit>
  <iSampleRate>22050</iSampleRate>
  <iSampleBits>16</iSampleBits>
  <iMultiChannelPref>2</iMultiChannelPref>
  <iNum2DSamples>64</iNum2DSamples>
  <iNum3DSamples>64</iNum3DSamples>
  <iNum2DStreams>10</iNum2DStreams>
  <iNum3DStreams>0</iNum3DStreams>
  <fPercentSamplesFor3D>0.6</fPercentSamplesFor3D>
 </AudioSystemInit>
|}

{{Civ4_XML_Files}}