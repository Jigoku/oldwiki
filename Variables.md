# Game Variables

<h4>
*Creating Custom Modes and Weapons*

</h4>
Red Eclipse offers a vast set of game variables to the user, allowing for extensive customization of settings as well as the creation of new weapons and modes. All of these variables can be accessed through the [console](Map::console "wikilink") and can be changed in-game real-time, both off and online.

# General Information

*To save changes to all variables during a match:*

`/writevars filename.cfg`

*To execute a set of custom variables:*

`/exec filename.cfg`

*To reset all variables in the current match:*

`/resetvars`

## Index of Terms

-   **"Inventory"** - consists of the weapon bar, impulse meter, health bar, and the "team" icon.

<!-- -->

-   **"Events"** - refer to the kill styles. Headshot, Dominating, Vengful, Carnage, Massacre, Bloodbath, 2x, 3x, and Multi-Kill are all "events". In odd/rare occaisions, this does NOT include Critical and First Blood.

<!-- -->

-   **"Notices"** - refer to the messages at the bottom center of the screen that tell you to pick up weapons, when you get frags, when you get fragged, etc.

<!-- -->

-   **"Indicator"** - This is the reload texture, the little progress circle that appears around your crosshair. It is also the "power" indicator for cooked grenades, or charged weapons.

<!-- -->

-   **"VAR\_MAX"** - This refers to game code. It is a macro for whatever the maximum integer amount the devs decide, which could be anything at any future point in development. For right now, even though I don't foresee any reason why you would need to be anywhere close to this value, VAR\_MAX is equal to: 2,147,483,646

<!-- -->

-   **"Tones"** - Tones change the color of certain HUD and model elements depending on certain parameters. All tones have "tone effects", that can do various things like *substitute 0x000000 with current weapon color*. These guidelines are the always the same, no matter what element; whether or not it's inventory color, or player color, or anything else.

The tones are as follows:

<table width="100%" border="1px" cellspacing="3" cellpadding="3">
<tr>
<th>
Value \#

</th>
<th>
TONE enum

</th>
<th>
Neutral (No teams)

</th>
<th>
Team Match

</th>
<th>
Mixed with

</th>
<th>
Description

</th>
<tr>
<tr>
<td>
-1

</td>
<td>
**N/A**

</td>
<td>
**Absolute** Profile color

</td>
<td>
**Absolute** Profile color

</td>
<td>
**N/A**

</td>
<td>
Use absolute profile color. Overrides team color in all cases. **Does not use any tone effects at all** (ie. Can therefore allow you to use 0x000000 as a color).

<td>
</tr>
<tr>
<td>
0

</td>
<td>
CTONE\_TEAM

</td>
<td>
**teamneutralcolor**

</td>
<td>
Current team color

</td>
<td>
None

</td>
<td>
Use team color (Includes neutral).

</td>
</tr>
<tr>
<td>
1

</td>
<td>
CTONE\_TONE

</td>
<td>
Profile color

</td>
<td>
Profile color

</td>
<td>
None

</td>
<td>
Uses profile color **regardless of team**.

</td>
</tr>
<tr>
<td>
2

</td>
<td>
CTONE\_TEAMED

</td>
<td>
Profile color

</td>
<td>
Current team color

</td>
<td>
None

</td>
<td>
Uses Profile color when Neutral, and team color when on any other team.

</td>
</tr>
<tr>
<td>
3

</td>
<td>
CTONE\_ALONE

</td>
<td>
**teamneutralcolor**

</td>
<td>
Profile color

</td>
<td>
None

</td>
<td>
Uses Neutral color when Neutral, and Profile color when on a team.

</td>
</tr>
<tr>
<td>
4

</td>
<td>
CTONE\_MIXED

</td>
<td>
**teamneutralcolor**

</td>
<td>
Current team color

</td>
<td>
Profile color

</td>
<td>
Uses Profile color, but "mixes" with your current team color, **including** neutral. With default Neutral color, this results in a "washed out" color.

</td>
</tr>
<tr>
<td>
5

</td>
<td>
CTONE\_TMIX

</td>
<td>
None

</td>
<td>
Current team color

</td>
<td>
Profile color

</td>
<td>
Uses Profile color, but "mixes" with your current team color. Will **NOT** mix Neutral.

</td>
</tr>
<tr>
<td>
6

</td>
<td>
CTONE\_AMIX

</td>
<td>
**teamneutralcolor**

</td>
<td>
None

</td>
<td>
Profile color

</td>
<td>
Uses profile color, but only in Team games (overrides team color). Mixes Neutral color with profile color when Neutral.

</tr>
</table>

