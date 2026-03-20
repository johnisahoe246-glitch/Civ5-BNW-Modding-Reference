Ready to create a new page detailing the tags in an XML file?  Just copy & paste the below code into any new XML reference page as a starting point.

Please remember, list your tags first by tag type as indicated below, and then ''alphabetically''.  This is a reference site, and not everyone is familiar with the sometimes confusing order Firaxis uses for the tags.

<pre>
The '''FILENAME''' file <<INSERT PURPOSE HERE>>.

All tags must be opened and closed; the first is the "open", the second the "close" tag. If nothing goes inside a "list tag", then it should just be the opening tag with a "/" before the closing bracket. The following tables contain all available tags, as well as their purpose and accepted values. 

<font color=red>This page is missing information.
Do not remove this notice until it is complete.</font>


==Tags==
===Headers===

These tags typically bracket other tags, sometimes the entire file, and are generally used to specify more than one piece of data.

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!Tag name
|enter text here
|-
!Tag name
|enter text here
|}


===Text===

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!Tag name
|enter text here
|-
!Tag name
|enter text here
|}


===Integers===

All of these tags have a numerical value.  Though it sometimes can be negative, it usually is not.

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!Tag name
|enter text here
|-
!Tag name
|enter text here
|}


===Boolean===

All of these can either be 1 (on, or true) or 0 (off, or false).  Be careful, as you can wind up with a double-negative, which the game will interpret as "True".

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!Tag name
|enter text here
|-
!Tag name
|enter text here
|}


===Lists (Multi-line)===

All List tags consist of an opening/closing tag, which is shown here, and then each entry within it is another tag with the same name as the parent tag, minus the "s" (i.e. singular, rather than plural).

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!Tag name
|enter text here
|-
!Tag name
|enter text here
|}


===Art===

These tags are directly related to the rendering of art for the entry.

{| border="1" style="text-align:left" cellpadding="3" cellspacing="0"
|-
! style="background:#efefef;" | Tag Name
! style="background:#efefef;" | Description
|-
!Tag name
|enter text here
|-
!Tag name
|enter text here
|}


==Example==

In the following example of code, please note that there is a specific order of all of the tags.  You ''must'' list the tags in this order for the game to properly interpret your file.

  <insert code example from actual XML file>

{{Civ4_XML_Files}}
</pre>