==CIV5UnitMovementRates.xml==
*The CIV5UnitMovementRates.xml file contains definitions for how movement is handled for various types of units. 
*The tables below indicate the structure of the entries in the CIV5UnitMovementRates file.
*This information is taken from the CIV5UnitMovementRates.xml file itself.

==MovementRates==
*This table is referenced by [[CIV5Units]] Units table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ MovementRates Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | NotNull
|-
| Type || Text || True
|-
| NumHexes || Integer || True
|-
| TotalTime || Float || 
|-
| EaseIn || Float || 
|-
| EaseOut || Float || 
|-
| IndividualOffset || Float || 
|-
| RowOffset || Float || 
|-
| CurveRoll || Float || 
|-
| PathSubdivision || Integer || 
|}

{{Civ5_XML_Files}}