{{Civ5 API Beta Banner}}
''This page is a part of the [[Lua and UI Reference (Civ5)]].''<br/>



=New Properties=
{{PseudoH4|BoxButton}}
:Format: Unknown.
:Usage: Unknown.


=Inherited from ButtonBase=
''XML Properties:'' <code>{{PropLabel5|Void1}}{{PropLabel5|Void2}}</code>
{|cellspacing="4" cellpadding="0" width="100%" 
|-
| [[File:Civ5-16.png|Base game]] || [[File:GK.png|Gods &amp; Kings]] || || || <code style="visibility:hidden;">___________________________</code>
<!-- 
CLEARCALLBACK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|ClearCallback}}<b>(</b>{{Type5|MouseType}} arg0<b>)</b></code>
<!-- 
ISTRACKINGMIDDLEMOUSEBUTTON
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|IsTrackingMiddleMouseButton}}<!-- No arguments --></code>
<!-- 
ISTRACKINGRIGHTMOUSEBUTTON
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{UnknownSignature5}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|IsTrackingRightMouseButton}}<!-- No arguments --></code>
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
GETVOID1
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ActionType}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetVoid1}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
GETVOID2
-->
|-
{{FuncInfos5|maybe|maybe|no |<!-- No comment -->}}
|align="right"  |<code>{{Type5|ResourceType}}</code>
|width="100%" |<code>{{FuncLabel5|UIElement|GetVoid2}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
ISTRACKINGLEFTMOUSEBUTTON
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code>'''bool'''</code>
|width="100%" |<code>{{FuncLabel5|UIElement|IsTrackingLeftMouseButton}}<b>(</b><!-- No arguments --><b>)</b></code>
<!-- 
REGISTERCALLBACK
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|RegisterCallback}}<b>(</b>{{Type5|MouseType}} OnSearchTextEnter, ('''void''' func<b>(</b>{{Type5|PolicyBranchType}} policyBranchIndex, {{Type5|UnitType}} y, {{Type5|Button}} button<b>)</b>) OnClose = nil<b>)</b></code>
<!-- 
SETVOID1
-->
|-
{{FuncInfos5|yes  |yes  |no |<!-- No comment -->}}
|align="right"  |<code><!-- No return type --></code>
|width="100%" |<code>{{FuncLabel5|UIElement|SetVoid1}}<b>(</b>{{Type5|OrderType}} MAINTAIN_GOLD<b>)</b></code>
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
''Redundant occurences have been removed.''

{{PseudoH4|MPList.xml}}
:<code>UI/InGame/WorldView/MPList.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0022}}<syntaxhighlight lang="xml"><BoxButton Anchor="R,T" Size="200,30" Color="0,0,0,0" ID="TeamClickEntry"/></syntaxhighlight>
{{CodeBreak5}}
{{CodeLine5|0041}}<syntaxhighlight lang="xml"><BoxButton Anchor="R,T" Size="200,28" Color="0,0,0,0" ID="ClickEntry"/></syntaxhighlight>
{{CodeEnd5}}


{{PseudoH4|Styles.xml}}
:<code>UI/Styles.xml</code>
:{{CodeBegin5}}
{{CodeLine5|0077}}<syntaxhighlight lang="xml"><BoxButton ></syntaxhighlight>
{{CodeEnd5}}




{{Civ5 API Footer}}
[[Category:Civ5 Types|BoxButton]]