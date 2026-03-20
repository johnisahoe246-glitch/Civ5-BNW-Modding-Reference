''This page is a part of the [[Lua and UI Reference (Civ5)]].''

= ButtonBase =
== Voids ==
<h4>Void1</h4>
:Format: any integer.
:Usage: This value is passed to the registered callbacks for user inputs (such as a click) and can be used in Lua to associate a control with the corresponding data.


<h4>Void2</h4>
:Same as [[#Void1]].

= AnimBase =
== Animation behavior ==
<h4>Stopped</h4>
:Format: <code>0</code> or <code>1</code>.
:Usage: 

<h4>Pause</h4>
:Format: any positive floating point.
:Usage: 

<h4>EndPause</h4>
:Format: any positive floating point.
:Usage:

<h4>Cycle</h4>
:Format: <code>Once</code> or <code>Bounce</code>.
:Usage: 

== Speed and acceleration ==
<h4>Speed</h4>
:Format: any positive floating point..
:Usage: 

<h4>Function</h4>
:Format: <code>Root</code> or <code>Square</code>.
:Usage: 

<h4>FunctionPower</h4>
:Format: any positive floating point.
:Usage:

= TextBase =

== Text and font ==
<h4>String</h4>
:Format: any string. May be a text key.
:Usage: The text to be displayed.

<h4>Font</h4>
:Format: <code>TwCenMT14</code>, <code>TwCenMT16</code>, <code>TwCenMT18</code>, <code>TwCenMT20</code>, <code>TwCenMT22</code>, or <code>TwCenMT24</code>.
:Usage: The font name and size used to render the text. 

<h4>FontStyle</h4>
:Format: <code>Base</code>, <code>Shadow</code>, <code>SoftShadow</code>, <code>Stroke</code> or an empty string.
:Usage: The style to apply to the text.

== Font color ==
<h4>ColorSet</h4>
:Format: any of the color sets defined in <code>Assets/UI/ColorAtlas.xml</code>. Typical values are <code>Beige_Black_Alpha</code> or <code>Beige_Black</code>.
:Usage: 

<h4>Color0</h4>
:Format: see [[#Color]]
:Usage: 

<h4>Color1</h4>
:Format: see [[#Color]].
:Usage: 

<h4>Color2</h4>
:Format: see [[#Color]]. 
:Usage: 

<h4>Color3</h4>
:Format: see [[#Color]].
:Usage:

== Text layout ==
<h4>WrapWidth</h4>
:Format: any integer.
:Usage: 

<h4>TruncateWidth</h4>
:Format: any integer. 
:Usage: 

<h4>ReduceOnTruncate</h4>
:Format: any integer.
:Usage: 

<h4>LeadingOffset</h4>
:Format: any integer.
:Usage:

== Input method editor ==
<h4>ForceIME</h4>
:Format: <code>0</code> or <code>1</code>.
:Usage: 

<h4>ForceNonIME</h4>
:Format: <code>0</code> or <code>1</code>.
:Usage:

= ControlBase =
== Core properties ==
<h4>ID</h4>
:Format: any string.
:Usage: 

<h4>Disabled</h4>
:Format: <code>0</code> or <code>1</code>.
:Usage:

== Appearance ==
<h4>Hidden</h4>
:Format: <code>0</code> or <code>1</code>.
:Usage: 

<h4>Style</h4>
:Format: the name of a style defined in <code>Assets/UI/Styles.xml</code>.
:Usage: 

<h4>NoClip</h4>
:Format: <code>0</code> or <code>1</code>.
:Usage: 

<h4>Color</h4>
:Format: either <code>R,G,B,A</code> or <code>Color, A</code>. Examples: <code>255,0,0,128</code> or <code>Red,128</code>.
:*''Color'' is one of the color names defined in <code>Assets/UI/ColorAtlas.xml</code> or in the {{Table5|Colors|Civ5Colors}} table.
:*''R'', ''G'', ''B'' and ''A'' are integer values between 0 and 255. The alpha parameter is optional.
:*Separators may be dots or commas.
:Usage: 

<h4>BranchAlpha</h4>
:Format: any positive floating point.
:Usage:

== Layout ==
[[File:Anchoring.png|frame|right|Different anchoring combinations for a child within its parent container. Size and offset are constant for all positions.]]
<h4>Size</h4>
:Format: <code>X,Y</code> where X and Y are positive integers. The separator may be a dot or a comma.
:Usage: 

<h4>Offset</h4>
:Format: <code>X,Y</code> where X and Y are positive integers. The separator may be a dot or a comma.
:Usage: 

<h4>Anchor</h4>
:Format: <code>X,Y</code>. The separator may be a dot or a comma.
:*X may be <code>Left</code>, <code>Center</code>, <code>Right</code>, <code>L</code>, <code>C</code> or <code>R</code>.
:*Y may be <code>Top</code>, <code>Center</code>, <code>Bottom</code>, <code>T</code>, <code>C</code> or <code>B</code>.
:*The character case does not matter.
:Usage: 

<h4>AnchorSide</h4>
:Format: <code>X,Y</code> where X and Y are either <code>i</code> or <code>o</code>. The separator may be a dot or a comma.
:*The possible values stand for "inner" and "outer".
:*The character case does not matter.
:Usage:

== Interaction ==

<h4>NeedsMouseOver</h4>
:Format: <code>0</code> or <code>1</code>.
:Usage: 

<h4>ConsumeMouse</h4>
:Format: <code>0</code> or <code>1</code>.
:Usage: 

<h4>ConsumeMouseOver</h4>
:Format: <code>0</code> or <code>1</code>.
:Usage: 

<h4>ConsumeMouseWheel</h4>
:Format: <code>0</code> or <code>1</code>.
:Usage: 

<h4>ConsumeMouseButton</h4>
:Format: <code>0</code> or <code>1</code>.
:Usage:

== Tool tips ==
<h4>ToolTip</h4>
:Format: any string.
:Usage: 

<h4>ToolTipType</h4>
:Format: any string, the name of a previously defined {{Type5|ToolTipType}}.
:Usage:

[[Category:Civ5 API]]