{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



{{TypeInfos5|Braces.png|This object is defined in the following Lua source file: ''InstanceManager.lua''.
:To import it, use: <code>include("InstanceManager")</code>}}


=Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a '''colon''', as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of InstanceManager.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, &lt;args&gt;)</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
BUILDINSTANCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|InstanceManager|BuildInstance}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETINSTANCE
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown'''</code>
|width="100%" |<code>{{FuncLabel5|InstanceManager|GetInstance}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
NEW
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|InstanceManager}}</code>
|width="100%" |<code>{{FuncLabel5|InstanceManager|new}}<b>(</b>'''string''' instanceName, '''string''' instanceRootName, '''ControlBase''' hostControl<b>)</b></code>
<!-- 
RELEASEINSTANCE
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|InstanceManager|ReleaseInstance}}<b>(</b>'''table''' instance<b>)</b></code>
<!-- 
RESETINSTANCES
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|InstanceManager|ResetInstances}}<b>(</b><!-- No arguments --><b>)</b></code>
|}


=Used by=
{|cellspacing="4" cellpadding="0" width="100%" style="background-color:#F0F0F0"
<!-- 
NEW
-->
|-
|align="right" width="200" |<code>{{Type5|InstanceManager}}</code>
|style="padding-left:6px" |<code>{{Type5|InstanceManager}}:{{Func5|InstanceManager|new}}<b>(</b>'''string''' instanceName, '''string''' instanceRootName, '''ControlBase''' hostControl<b>)</b></code>
|}




{{Civ5 API Footer}}
[[Category:Civ5 Types|InstanceManager]]