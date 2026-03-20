{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



= Usage =
* {{Lua}} Contexts are defined through the <code>&lt;Context&gt;</code> XML tag. They are the root of every UI file.
* {{Lua}} They are linked in another context through the <code>&lt;LuaContext&gt;</code> XML tag.
* {{UI}} A global Lua object is associated with the current context: <code>ContextPtr</code>
* {{UI}} Another global Lua object, <code>Controls</code>, stores all the controls defined in the XML file, provided they have an ID associated with them.


== Contexts are UI parts, but not reusable components ==
Contexts are static parts of the UI. They are used to split the UI into different files.


You can nest one context into another through <code>LuaContext</code>. With the following example, the new context will appear in the current one under <code>Controls.LegalScreen</code> and will behave as a new control.
<syntaxhighlight lang="xml" class="civ5-example">
	<!-- This includes in this context a context defined in another file. This new context will behave as a control and will be stored under Controls.LegalScreen -->
	<LuaContext FileName="Assets/UI/FrontEnd/LegalScreen" ID="LegalScreen"/>
</syntaxhighlight>


Now contexts cannot be efficiently used as a way to implement reusable controls because of the isolation explained in the next section. While LuaEvents could be used to circumvent this isolation, it's not really suited to instancing. The main point of Lua contexts is just to split your UI into different files and to provide an isolation mechanism.


== Contexts are isolation scopes ==
But UI contexts are not just parts of the UI. They also represent contexts in the meaning defined in Lua. 


Lua contexts are static (non-instanced) isolation scopes. That is, a Lua variable defined in one context is not visible from other contexts. However some things are shared across contexts:
* Any {{Type5|Instance}} defined in a context is visible in children contexts and further descendants.
* The data tables, styles and colors are visible from all contexts and have the same value in all those contexts.
* The events declared on {{Type5|LuaEvents}} are visible in all contexts and they are the only way to achieve inter-contexts communication and objects and tables across contexts.


Finally, while the game state is always the same in all contexts, the API objects are specific to every context. That is, if you try for example to compare a {{Type5|Player}} instance from one context with the same instance from the current context, the result will be false because they are different objects.
<syntaxhighlight lang="lua" class="civ5-example">
return pIndianPlayerFromContext1 == pIndianPlayerFromContext1 -- returns true
return pIndianPlayerFromContext1 == pIndianPlayerFromContext2 -- returns false
return pIndianPlayerFromContext1:GetCivilizationType() == pIndianPlayerFromContext2:GetCivilizationType() -- returns true
</syntaxhighlight>


== Contexts all execute on the same thread ==
A common misconception is that contexts are ran in different threads. This is absolutely wrong. Actually, Civ5 is almost a purely mono-threaded game since everything from the rendering to the Lua execution and the game logic all run on a single thread. As a result all contexts are executed one after the other and a mod can block the UI and make the game hang, for example through an infinite loop. 

So if you need to perform long-running computations, you need to split this task into multiple parts (Lua coroutines may be used for that purpose) and run one part anytime the update callback is invoked (see [[#Update]]).


=New Properties=
{{PseudoH4|Color0}}
:Format: Unknown.
:Usage: Unknown.


{{PseudoH4|Color1}}
:Format: Unknown.
:Usage: Unknown.


{{PseudoH4|ColorSet}}
:Format: Unknown.
:Usage: Unknown.


{{PseudoH4|Context}}
:Format: Unknown.
:Usage: Unknown.


{{PseudoH4|DeferLoad}}
:Format: Unknown.
:Usage: Unknown.


{{PseudoH4|FileName}}
:Format: Unknown.
:Usage: Unknown.


{{PseudoH4|Font}}
:Format: Unknown.
:Usage: Unknown.


{{PseudoH4|FontStyle}}
:Format: Unknown.
:Usage: Unknown.


{{PseudoH4|Name}}
:Format: Unknown.
:Usage: Unknown.


=New Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a colon, as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of Context.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, ''&lt;args&gt;'')</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
BUILDINSTANCE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|BuildInstance}}<b>(</b>'''string''' arg0, '''table''' arg1<b>)</b></code>
<!-- 
BUILDINSTANCEFORCONTROL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|BuildInstanceForControl}}<b>(</b>'''string''' arg0, '''table''' arg1, {{Type5|Stack}} arg2<b>)</b></code>
<!-- 
BUILDINSTANCEFORCONTROLATINDEX
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|BuildInstanceForControlAtIndex}}<b>(</b>'''string''' arg0, '''table''' controlTable, {{Type5|Stack}} arg2, '''int''' arg3<b>)</b></code>
<!-- 
CALLPARENTSHOWHIDEHANDLER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|CallParentShowHideHandler}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
CALLSHOWHIDEHANDLER
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|CallShowHideHandler}}<!-- No arguments --></code>
<!-- 
CLEARUPDATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|ClearUpdate}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
DODEFERREDLOAD
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|DoDeferredLoad}}<!-- No arguments --></code>
<!-- 
ISHOTLOAD
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UIElement|IsHotLoad}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
LOADNEWCONTEXT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Context}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|LoadNewContext}}<b>(</b>'''string''' path<b>)</b></code>
<!-- 
LOOKUPCONTROL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Container}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|LookUpControl}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
RELOAD
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|Reload}}<!-- No arguments --></code>
<!-- 
SETINPUTHANDLER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetInputHandler}}<b>(</b>('''void''' func<b>(</b>{{Type5|MouseEventType}} uiMsg, {{Type5|KeyType}} wParam, '''unknown''' lParam<b>)</b>) InputHandler<b>)</b></code>
<!-- 
SETPOSTINIT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetPostInit}}<!-- No arguments --></code>
<!-- 
SETSHOWHIDEHANDLER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetShowHideHandler}}<b>(</b>('''void''' func<b>(</b>'''bool''' isHide, '''int''' bInitState<b>)</b>) ShowHide<b>)</b></code>
<!-- 
SETSHUTDOWN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetShutdown}}<b>(</b>('''void''' func<b>(</b><b>)</b>) OnShutdown<b>)</b></code>
<!-- 
SETUPDATE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetUpdate}}<b>(</b>('''void''' func<b>(</b>'''float''' fTimeDelta<b>)</b>) UpdateHandler<b>)</b></code>
<!-- 
SETTEXTUREOFFSET
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetTextureOffset}}<b>(</b>{{Type5|Vector2}} questionOffset<b>)</b></code>
|}


=Inherited from ControlBase=
''XML Properties:'' <code>''none.''</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
BUILDENTRY
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|BuildEntry}}<b>(</b>'''string''' arg0, '''table''' arg1<b>)</b></code>
<!-- 
CALCULATEINTERNALS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|CalculateInternals}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CALCULATEINTERNALSIZE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|CalculateInternalSize}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CALCULATESIZE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|CalculateSize}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CLEARENTRIES
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|ClearEntries}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETBUTTON
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Button}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetButton}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
REGISTERCHECKHANDLER
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|RegisterCheckHandler}}<b>(</b>('''void''' func<b>(</b>'''bool''' bIsChecked<b>)</b>) OnPolicyInfo<b>)</b></code>
<!-- 
REGISTERSELECTIONCALLBACK
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|RegisterSelectionCallback}}<b>(</b>('''void''' func<b>(</b>{{Type5|FaithPurchaseType}} v1, '''int''' v2<b>)</b>) OnChatTarget<b>)</b></code>
<!-- 
SETCHECK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetCheck}}<b>(</b>'''bool''' cityBanners<b>)</b></code>
<!-- 
SETPERCENT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetPercent}}<b>(</b>'''int''' percentDone<b>)</b></code>
<!-- 
SETPERCENTS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetPercents}}<b>(</b>'''float''' productionProgressPercent, '''float''' productionProgressPlusThisTurnPercent<b>)</b></code>
<!-- 
SETSCROLLVALUE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetScrollValue}}<b>(</b>'''int''' arg0<b>)</b></code>
<!-- 
SETTEXTURE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetTexture}}<b>(</b>'''string''' textureName<b>)</b></code>
<!-- 
SETTEXTUREOFFSETVAL
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetTextureOffsetVal}}<b>(</b>'''int''' arg0, '''int''' offset<b>)</b></code>
<!-- 
UNLOADTEXTURE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|UnloadTexture}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETVOID2
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetVoid2}}<b>(</b>{{Type5|ProcessType}} process<b>)</b></code>
<!-- 
SETVOIDS
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetVoids}}<b>(</b>{{Type5|ResourceType}} building, {{Type5|ResourceType}} addToList<b>)</b></code>
<!-- 
GETTEXT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetText}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
LOCALIZEANDSETTEXT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|LocalizeAndSetText}}<b>(</b>'''string''' name, '''int''' searchString = nil, '''string''' minFaithForProphet = nil, '''unknown''' arg3, '''unknown''' arg4, '''unknown''' arg5, '''unknown''' arg6, '''unknown''' arg7, '''unknown''' arg8, '''string''' arg9, '''unknown''' arg10, '''unknown''' arg11<b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} OnSearchTextEnter, ('''void''' func<b>(</b>{{Type5|PolicyBranchType}} policyBranchIndex, {{Type5|UnitType}} y, {{Type5|Button}} button<b>)</b>) OnClose = nil<b>)</b></code>
<!-- 
SETTEXT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetText}}<b>(</b>'''string''' localizedString<b>)</b></code>
<!-- 
SETVOID1
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetVoid1}}<b>(</b>{{Type5|OrderType}} MAINTAIN_GOLD<b>)</b></code>
|}


==Common==
''XML Properties:'' <code>{{PropLabel5|ID}}{{PropLabel5|Disabled}}</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CHANGEPARENT
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|ChangeParent}}<b>(</b>{{Type5|Image}} parent<b>)</b></code>
<!-- 
DESTROYALLCHILDREN
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|DestroyAllChildren}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETID
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetID}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETNUMCHILDREN
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetNumChildren}}<!-- No arguments --></code>
<!-- 
ISDISABLED
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|IsDisabled}}<!-- No arguments --></code>
<!-- 
RELEASECHILD
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|ReleaseChild}}<b>(</b>{{Type5|WorldAnchor}} arg0<b>)</b></code>
<!-- 
SETDISABLED
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetDisabled}}<b>(</b>'''bool''' disableBanners<b>)</b></code>
<!-- 
SORTCHILDREN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SortChildren}}<b>(</b>('''void''' func<b>(</b>'''unknown''' a, '''unknown''' b<b>)</b>) SortFunction<b>)</b></code>
|}


==Layout==
''XML Properties:'' <code>{{PropLabel5|Size}}{{PropLabel5|Offset}}{{PropLabel5|Anchor}}{{PropLabel5|AnchorSide}}</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETOFFSETVAL
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''unknown''', '''int'''</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetOffsetVal}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETOFFSETX
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetOffsetX}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETOFFSETY
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetOffsetY}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSIZE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|Vector2}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetSize}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSIZEVAL
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''int''', '''int'''</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetSizeVal}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSIZEX
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetSizeX}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETSIZEY
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetSizeY}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
REPROCESSANCHORING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|ReprocessAnchoring}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETANCHOR
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetAnchor}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
SETOFFSET
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetOffset}}<b>(</b>{{Type5|Vector2}} offset<b>)</b></code>
<!-- 
SETOFFSETVAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetOffsetVal}}<b>(</b>'''int''' xOffset, '''int''' yOffset<b>)</b></code>
<!-- 
SETOFFSETX
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetOffsetX}}<b>(</b>'''int''' xOffset<b>)</b></code>
<!-- 
SETOFFSETY
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetOffsetY}}<b>(</b>'''int''' TOP_COMPENSATION<b>)</b></code>
<!-- 
SETSIZE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetSize}}<b>(</b>'''table''' blockSize<b>)</b></code>
<!-- 
SETSIZEVAL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetSizeVal}}<b>(</b>'''int''' baseWidth, '''int''' newHeight<b>)</b></code>
<!-- 
SETSIZEX
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetSizeX}}<b>(</b>'''int''' width<b>)</b></code>
<!-- 
SETSIZEY
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetSizeY}}<b>(</b>'''int''' newSizeY<b>)</b></code>
|}


==Appearance==
''XML Properties:'' <code>{{PropLabel5|Hidden}}{{PropLabel5|Style}}{{PropLabel5|NoClip}}{{PropLabel5|Color}}{{PropLabel5|BranchAlpha}}</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
BRANCHRESETANIMATION
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|BranchResetAnimation}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
CALCULATEVISIBILITYBOX
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|CalculateVisibilityBox}}<!-- No arguments --></code>
<!-- 
ISHIDDEN
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''int'''</code>
|width="100%" |<code>{{FuncLabel5|UIElement|IsHidden}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETALPHA
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetAlpha}}<b>(</b>'''float''' DimAlpha<b>)</b></code>
<!-- 
SETCOLOR
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetColor}}<b>(</b>'''table''' fadeColor, '''int''' arg1<b>)</b></code>
<!-- 
SETCOLORBYNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetColorByName}}<b>(</b>'''string''' colorSet<b>)</b></code>
<!-- 
SETCOLORCHANNEL
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetColorChannel}}<b>(</b>'''int''' arg0, '''float''' arg1<b>)</b></code>
<!-- 
SETCOLORVAL
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetColorVal}}<b>(</b>'''int''' arg0, '''int''' arg1 = nil, '''int''' arg2 = nil, '''int''' arg3 = nil<b>)</b></code>
<!-- 
SETHIDE
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetHide}}<b>(</b>'''int''' disablePolicies<b>)</b></code>
<!-- 
SETNOCLIP
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetNoClip}}<!-- No arguments --></code>
|}


==Interaction==
''XML Properties:'' <code>{{PropLabel5|NeedsMouseOver}}{{PropLabel5|ConsumeMouse}}{{PropLabel5|ConsumeMouseOver}}{{PropLabel5|ConsumeMouseWheel}}{{PropLabel5|ConsumeMouseButton}}</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETCONSUMEMOUSEBUTTON
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetConsumeMouseButton}}<!-- No arguments --></code>
<!-- 
GETCONSUMEMOUSEOVER
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetConsumeMouseOver}}<!-- No arguments --></code>
<!-- 
GETCONSUMEMOUSEWHEEL
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetConsumeMouseWheel}}<!-- No arguments --></code>
<!-- 
HASMOUSEOVER
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UIElement|HasMouseOver}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETCONSUMEMOUSEBUTTON
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetConsumeMouseButton}}<!-- No arguments --></code>
<!-- 
SETCONSUMEMOUSEOVER
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetConsumeMouseOver}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
SETCONSUMEMOUSEWHEEL
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetConsumeMouseWheel}}<!-- No arguments --></code>
|}


==Tool Tip==
''XML Properties:'' <code>{{PropLabel5|ToolTip}}{{PropLabel5|ToolTipType}}</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
ENABLETOOLTIP
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|EnableToolTip}}<b>(</b>'''bool''' arg0<b>)</b></code>
<!-- 
GETTOOLTIPSTRING
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetToolTipString}}<!-- No arguments --></code>
<!-- 
ISTOOLTIPENABLED
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|IsToolTipEnabled}}<!-- No arguments --></code>
<!-- 
LOCALIZEANDSETTOOLTIP
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|LocalizeAndSetToolTip}}<b>(</b>'''string''' description, '''string''' minFaithForProphet = nil, '''string''' threshold, '''string''' moodText, '''string''' spyRank, '''string''' spyName, '''string''' spyRank, '''string''' spyName, '''unknown''' arg8, '''unknown''' arg9, '''string''' arg10, '''unknown''' arg11, '''unknown''' arg12<b>)</b></code>
<!-- 
SETTOOLTIPCALLBACK
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetToolTipCallback}}<b>(</b>('''void''' func<b>(</b>{{Type5|Slider}} control<b>)</b>) TipHandler<b>)</b></code>
<!-- 
SETTOOLTIPSTRING
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetToolTipString}}<b>(</b>'''string''' foodToolTip<b>)</b></code>
<!-- 
SETTOOLTIPTYPE
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetToolTipType}}<b>(</b>'''string''' arg0<b>)</b></code>
|}


=Source code samples=
''Too many occurences. Only 10 out of 517 are listed.''

{{PseudoH4|EmptyPopup.xml}}
:<code>UI/InGame/Popups/EmptyPopup.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0002}}<syntaxhighlight lang="xml"><Context/></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|FrontEnd.xml}}
:<code>UI/FrontEnd/FrontEnd.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0002}}<syntaxhighlight lang="xml"><Context ColorSet="Beige_Black_Alpha" Font="TwCenMT22" FontStyle="Shadow" Name="FrontEnd" ></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|GameMenu.xml}}
:<code>UI/InGame/Menus/GameMenu.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0289}}<syntaxhighlight lang="xml"><LuaContext FileName="Assets/UI/InGame/Menus/SaveMapMenu" ID="SaveMapMenu" Hidden="True" /></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.xml}}
:<code>UI/InGame/InGame.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0041}}<syntaxhighlight lang="xml"><LuaContext FileName="Assets/UI/InGame/Popups/TechAwardPopup"         ID="TechAwardPopup"         Hidden="True" /></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|InGame.xml (G&K)}}
:<code>DLC/Expansion/UI/InGame/InGame.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0025}}<syntaxhighlight lang="xml"><LuaContext FileName="Assets/UI/InGame/Popups/GoodyHutPopup" ID="GoodyHutPopup" Hidden="True"/></syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0029}}<syntaxhighlight lang="xml"><LuaContext FileName="Assets/UI/InGame/Popups/CityStateGreetingPopup" ID="CityStateGreetingPopup" Hidden="True"/></syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0054}}<syntaxhighlight lang="xml"><LuaContext FileName="Assets/UI/InGame/TopPanel" ID="TopPanel"/></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MainMenu.xml}}
:<code>UI/FrontEnd/MainMenu.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0184}}<syntaxhighlight lang="xml"><LuaContext FileName="Assets/UI/FrontEnd/SinglePlayer" ID="SinglePlayerScreen" Hidden="1"/></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|NotificationPanel.xml}}
:<code>UI/InGame/WorldView/NotificationPanel.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0002}}<syntaxhighlight lang="xml"><Context  ></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|OtherMenu.xml}}
:<code>UI/FrontEnd/OtherMenu.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0118}}<syntaxhighlight lang="xml"><LuaContext FileName="Assets/UI/FrontEnd/LatestNews" ID="LatestNews" Hidden="1" DeferLoad="1"/></syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Context]]