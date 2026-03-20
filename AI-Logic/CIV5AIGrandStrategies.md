==CIV5AIGrandStrategies.xml==
*From the header of the xml file:
<blockquote>
AI Player Grand Strategy Infos                             
Entries in this file define the attributes of various      
AI Player Grand Strategies, which focus the AI player      
on the different Victory Competitions.  Entries can        
be completely removed safely if you don't want the AI      
to pursue a particular Grand Strategy/Victory              
Competition.  Defines which also help shape use of AI      
Player Grand Strategies are located in the                 
GlobalAIDefines.xml file inside the XML\AI\ directory.     
Flavors determine how likely an AI Player (with            
intrinsic Personality Flavors) is to adopt a               
particular Grand Strategy.  For more information on how    
these Grand Strategies work, reference                     
CvPlayerGrandStrategyAI.cpp in the GameCoreDLL project.    
</blockquote>

==AIGrandStrategies==
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ AIGrandStrategies Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Notes
|-
| ID || Integer || Primary Key, Autoincrement
|-
| Type || Text || Not Null, Unique
|}

==AIGrandStrategy_Flavors==
*[[CIV5Flavors]] contains the definitions of the Flavors used in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ AIGrandStrategy_Flavors Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| AIGrandStrategyType || Text || AIGrandStrategies(Type)
|-
| FlavorType || Text || Flavors(Type)
|-
| Flavor || Integer ||
|}

==AIGrandStrategy_Yields==
*[[CIV5Yields]] contains the definitions of the Yields used in this table.
{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"				
|+ AIGrandStrategy_Yields Table					
|-	
! scope="col" style="background: #efefef;" | Name	
! scope="col" style="background: #efefef;" | Type	
! scope="col" style="background: #efefef;" | Reference
|-
| AIGrandStrategyType || Text || AIGrandStrategies(Type)
|-
| YieldType || Text || Yields(Type)
|-
| Yield || Integer ||
|}

{{Civ5_XML_Files}}