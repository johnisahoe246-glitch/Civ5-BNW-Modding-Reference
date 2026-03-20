{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=New Properties=
{{PseudoH4|ColorLayer0}}
:Format: Unknown.
:Usage: Unknown.


{{PseudoH4|ColorLayer1}}
:Format: Unknown.
:Usage: Unknown.


{{PseudoH4|TextAnchor}}
:Format: Unknown.
:Usage: Unknown.


{{PseudoH4|TextAnchorSide}}
:Format: Unknown.
:Usage: Unknown.


=New Instance Methods=
Methods are functions that belong to an object. Instance methods are invoked through a colon, as in <code>caller:SomeMethod(&lt;args&gt;)</code>, where ''caller'' is an instance of Label.<br/>
A colon implictly passes the caller object as the first argument. That is, the former call is equivalent to this one: <code>caller.SomeMethod(caller, ''&lt;args&gt;'')</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
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
SETTEXT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetText}}<b>(</b>'''string''' localizedString<b>)</b></code>
|}


=Inherited from TextBase=
''XML Properties:'' <code>{{PropLabel5|String}}{{PropLabel5|Font}}{{PropLabel5|FontStyle}}{{PropLabel5|WrapWidth}}{{PropLabel5|TruncateWidth}}{{PropLabel5|ReduceOnTruncate}}{{PropLabel5|LeadingOffset}}{{PropLabel5|ColorSet}}{{PropLabel5|Color0}}{{PropLabel5|Color1}}{{PropLabel5|Color2}}{{PropLabel5|Color3}}{{PropLabel5|ForceIME}}{{PropLabel5|ForceNonIME}}</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
GETTEXT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''string'''</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetText}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
SETFONTBYNAME
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetFontByName}}<b>(</b>'''string''' arg0<b>)</b></code>
<!-- 
SETFORCEIME
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetForceIME}}<!-- No arguments --></code>
<!-- 
SETFORCENONIME
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetForceNonIME}}<!-- No arguments --></code>
<!-- 
SETSTRING
-->
|-
{{FuncInfos5|maybe|yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetString}}<b>(</b>'''unknown''' arg0<b>)</b></code>
<!-- 
SETTRUNCATEWIDTH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetTruncateWidth}}<b>(</b>'''int''' width<b>)</b></code>
<!-- 
SETWRAPWIDTH
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetWrapWidth}}<b>(</b>{{Type5|PlayerID}} arg0<b>)</b></code>
<!-- 
LOCALIZEANDSETTEXT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|LocalizeAndSetText}}<b>(</b>'''string''' name, '''int''' searchString = nil, '''string''' minFaithForProphet = nil, '''unknown''' arg3, '''unknown''' arg4, '''unknown''' arg5, '''unknown''' arg6, '''unknown''' arg7, '''unknown''' arg8, '''string''' arg9, '''unknown''' arg10, '''unknown''' arg11<b>)</b></code>
<!-- 
SETTEXT
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetText}}<b>(</b>'''string''' localizedString<b>)</b></code>
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
''Too many occurences. Only 10 out of 3790 are listed.''

{{PseudoH4|AdvancedSetup.xml}}
:<code>UI/FrontEnd/GameSetup/AdvancedSetup.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0110}}<syntaxhighlight lang="xml"><Label Anchor="L,C" ColorSet="Beige_Black" Font="TwCenMT20" FontStyle="Shadow" String="TXT_KEY_AD_SETUP_HANDICAP" /></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|BarbarianCampPopup.xml}}
:<code>UI/InGame/Popups/BarbarianCampPopup.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0024}}<syntaxhighlight lang="xml"><Label Anchor="C,C" Offset="0,-2" String="TXT_KEY_CLOSE"  Color0="255.255.200.255" Color1="0.0.0.128" Color2="255.255.200.255" Font="TwCenMT22" FontStyle="Shadow" /></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|ChooseReligionPopup.xml (G&K)}}
:<code>DLC/Expansion/UI/InGame/Popups/ChooseReligionPopup.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0021}}<syntaxhighlight lang="xml"><Label Anchor="L,T" Offset="45,10" Font="TwCenMT20" ColorSet="Beige_Black_Alpha" FontStyle="Shadow" ID="Name"/></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityBannerManager.xml}}
:<code>UI/InGame/CityBannerManager.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0113}}<syntaxhighlight lang="xml"><Label ID="ResistanceIcon"  Anchor="C,C" Offset="0,0" String="[ICON_RESISTANCE]"    Hidden="1"/></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|CityView.xml}}
:<code>UI/InGame/CityView/CityView.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0072}}<syntaxhighlight lang="xml"><Label Anchor="C,T" Offset="0,18" String="TXT_KEY_CITYVIEW_CITYINFO_TEXT" ColorSet="Beige_Black_Alpha" Font="TwCenMT20" FontStyle="Shadow"/></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DebugMode.xml}}
:<code>UI/InGame/DebugMode.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0173}}<syntaxhighlight lang="xml"><Label Anchor="L,C" String="Unit Variable:"/></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|DiploRelationships.xml}}
:<code>UI/InGame/Popups/DiploRelationships.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0110}}<syntaxhighlight lang="xml"><Label ID="AllyLabel" Anchor="L,T" Offset="32,0" Font="TwCenMT14" FontStyle="Shadow" ColorSet="Beige_Black_Alpha" String="TXT_KEY_POP_CSTATE_ALLIED_WITH"></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Lobby.xml}}
:<code>UI/FrontEnd/Multiplayer/Lobby.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0025}}<syntaxhighlight lang="xml"><Label Anchor="C,C" Offset="0,0" Font="TwCenMT18" ColorSet="Beige_Black_Alpha" FontStyle="Shadow" ID="MembersLabel"/></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|MilitaryOverview.xml}}
:<code>UI/InGame/Popups/MilitaryOverview.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0138}}<syntaxhighlight lang="xml"><Label Offset="10,0" Font="TwCenMT18" Anchor="L,C" String="TXT_KEY_SUPPLY_REMAINING"  /></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|UITestMenu.xml}}
:<code>UI/FrontEnd/UITestMenu.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0126}}<syntaxhighlight lang="xml"><Label   Anchor="R,T"  Offset="30,10" ColorSet="Beige_Black" Font="TwCenMT18" FontStyle="Shadow" String="(M)" /></syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Types|Label]]