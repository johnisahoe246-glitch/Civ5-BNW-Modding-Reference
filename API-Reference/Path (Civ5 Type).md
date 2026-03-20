{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=Static Methods=
Methods are functions that belong to an object. Static methods are invoked through a '''dot''', as in <code>Path.SomeMethod(&lt;args&gt;)</code>. When a dot is used the caller object is not implicitly provided as the first argument.
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETALTDIRECTORYSEPARATORCHAR
-->
|-
{{FuncInfos5|maybe|maybe|yes|Retrieves an alternate directory separator character This method retrieves one of the two currently specified directory seperator characters used by paths '/'.}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Path|GetAltDirectorySeparatorChar}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETDIRECTORYNAME
-->
|-
{{FuncInfos5|maybe|maybe|yes|Returns a path to the deepest folder containing the target When used with paths to files, this method returns the folder containing the file.  When used with paths to directories, this method returns the folder containing the directory.}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Path|GetDirectoryName}}<b>(</b>'''string''' path<b>)</b></code>
<!-- 
GETDIRECTORYSEPARATORCHAR
-->
|-
{{FuncInfos5|maybe|maybe|yes|Gets the character used to seperate directories in a path. This method returns the character used to seperate directories in a path with ("\").}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Path|GetDirectorySeparatorChar}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETEXTENSION
-->
|-
{{FuncInfos5|yes  |yes  |yes|Returns the extension of a file This method returns the extension of a target file.  Returns an empty string if it cannot determine extension.}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Path|GetExtension}}<b>(</b>'''string''' path<b>)</b></code>
<!-- 
GETEXTENSIONSEPARATORCHAR
-->
|-
{{FuncInfos5|maybe|maybe|yes|Gets the character used to mark a file extension This method reutnrs the character used to begin a file extension in a path. "."}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|Path|GetExtensionSeparatorChar}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETFILENAME
-->
|-
{{FuncInfos5|maybe|maybe|yes|Gets the file name in the target path This method returns the complete filename in a path, including the extension.}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Path|GetFileName}}<b>(</b>'''string''' path<b>)</b></code>
<!-- 
GETFILENAMEWITHOUTEXTENSION
-->
|-
{{FuncInfos5|yes  |yes  |yes|Obtains the filename without the extension for a given path This method returns the name of the file, minus extension, in a given path.}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Path|GetFileNameWithoutExtension}}<b>(</b>'''string''' path<b>)</b></code>
<!-- 
GETPATHSEPARATORCHAR
-->
|-
{{FuncInfos5|maybe|maybe|yes|Grabs the character used to seperate multiple paths This returns the character used to separate multiple paths.}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Path|GetPathSeparatorChar}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETVOLUMESEPARATORCHAR
-->
|-
{{FuncInfos5|maybe|maybe|yes|Returns the character used to separate volumes in a path. This method returns the character used to separate volumes in a path. ":"}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Path|GetVolumeSeparatorChar}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
NORMALIZEPATH
-->
|-
{{FuncInfos5|maybe|maybe|yes|Returns a path in which all directory seperators are the same This method receives a path and returns the same path but with all directory separators set to use the character returned in Path.GetDirectorySeperatorChar().}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|Path|NormalizePath}}<b>(</b>'''string''' path<b>)</b></code>
<!-- 
USESEXTENSION
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|Path|UsesExtension}}<b>(</b>'''string''' file, '''string''' arg1<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Path]]