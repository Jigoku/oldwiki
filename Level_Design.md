Making a level that flows in Red Eclipse is a unique challenge: you have to balance the map to the weapons since they're not manually controlable via ammo like Quake, and the verticality of the player's motion means that special care in the flow of maps must be taken.

## "Flow" tips

-   Free for all and duel maps should not be symmetrical. Symmetrical maps inherently mean that both players can hold equally high ground; in a duel, two high grounds lends itself to a standoff.
-   Team maps should be symmetrical unless extreme levels of care are taken to balance the two different teams' strengths. (read: don't do it)
-   Try to make every room have three exits, and try to have the central room(s) ("atriums") have at least 4 exits.
-   Avoid vertical floor spacing of more than 64 cube units (8m); more than this will require a jump pad and will choke flow by forcing level changes through the jump pad.
-   Avoid rooms of larger than 64 meters in any direction; above this, players will burn lots of impulse to cross a featureless room. If you make rooms larger than this, adding geometry to break up the room or use of jumpers is advisable. Large rooms are boring to cross and difficult to texture well.
-   Most duel maps have one atrium where the action is concentrated; two or more atriums in a duel map can lead to a hide-and-seek match. Multi-atrium duel maps, however, can be superior to single-atrium maps if designed well, and are often necessary for large FFA matches to prevent them from becoming a mosh pit.
-   A jump pad is preferable to a teleporter if it is practical to implement.
-   Be very careful to establish visual cues when placing a teleporter; since going through one short-circuts the minimap layout, be sure to make it easy to identify the location teleporters exit into.
-   Stairs should have a slope of at least 2:3 or shallower; 2:1 is recommended whenever possible. 1:1 stairs are slow to climb, look ugly, and can jam a parkour slide.
-   The minimum width for a corridor should be 4 meters and the minimum height should be 5 meters. Any narrower and the player will be easily pinned down by rifle/smg/zapper fire; any shorter and the player feels cramped when trying to jump.
-   Do not place arbitrary clipping boundaries in places where players may be able to interact with them; very few things are more immersion breaking.
-   Careful use of sound and triggers, especially when linked to teleporters, helps establish aural cues to player position when they are out of sight. In Quake, positioning and quantity of shards is an important aural cue to player placement; while in RE this is not possible, carefully placed sound triggers can help duelists gain insight into the other player's whereabouts.

## Weapon balance tips

-   **Balancing all the different weapons is the most difficult part of making a Red Eclipse map. You cannot fix a weapon imbalance (particularly rifle) by counterbalancing the pickups like you can in Quake-style shooters. In Quake (and company), it is easy to balance a large, open map by making the pickups vulnerable to short range weapons. Red Eclipse rifle users are not under the same obligation to make themselves vulnerable.**
-   Try to avoid corridors or rooms of greater than 75 meters, especially without some way (vertical change, columns, snaking) to break up rifle fire. This is especially true in closed corridors, as opposed to open corridors running alongside a room.
-   On the other hand, maps should have one space of at least 40x20 meters in order not to totally exclude rifle usage. This corridor or room may be important, but try not to make it absolutely critical for movement across the map.
-   Be wary of adding a lot of mines in a map with a teleporter, as this can lead to excessive amounts of teleporter mining. Mines in excess in general are annoying as they not only shape gameflow but dominate it.
-   There should almost always be more grenades than mines on a map.
-   ***Never*** place more than one rocket on any map unless it is kaboom-only.

## Team-specific tips

-   Try to make multiple equally fast routes between bases to prevent a single path dominating the play style (ala *darkness*). Be sure that a base-to-base path has only marginally slower alternatives to allow a flag runner the ability to pick an unpredictable path.
-   Bases should not be exposed to 75+ meter lines of sight to increase the base's defensibility, and should never be directly visible from the other base.
-   The flag runner should be catchable from most of the map (e.g. an alpha player standing in a random spot on the map should be able to hit an omega flag runner before he reaches his base). Particularly important in implementing this is avoiding have base-to-base paths be totally seperate from each other; maps should not be shaped like a racetrack where there are only ever two directions to go.
-   Try to avoid having the flag runner be forced to run through a rifle corridor or open area; the runner is already at an inherent disadvantage due to the speed debuff and the bright flag carried on their back.
-   If possible, the fastest path between the bases should also be the least defensible and the easiest for a flag runner to be killed on.
-   Be aware that any deathmat or infinite cliff can be used to discard the flag and send it back to its original base.
-   Try to make the base-to-base time of any CTF map and the bomb-to-base time of any bomber ball map at least 10 seconds. Much shorter and it becomes difficult to stop someone from streaking into a base.

## Aesthetic considerations

-   Even if the justification for any particular piece of geometry or texturing is flimsy, as long as it doesn't look totally out of place, it will not break immersion.
-   Avoid creating a map based on a particular real-life object or place: almost never does it flow correctly in RE's nonstandard movement style. It is much better to make a good layout that requires some creative texturing than a good aesthetic design that cannot be morphed into a workable layout. Remember that a map's aesthetic is secondary to its primary purpose: to have players play on it.
-   In the same vein, gameplay and map flow trump aesthetic considerations. If necessary, use of clip and noclip can be used to mask minor aesthetic geometry changes.
-   If you have a low-powered laptop with integrated graphics, consider using it to ensure performance remains adequate on lower end machines. A map of 120-150k triangles should be easily possible on an e.g. HD 3000, but a low-end machine can expose inefficiencies that a well-speced rig would not catch. Compare performance to well-established geometry-heavy maps like Ghost or Deli if needed to confirm performance is acceptable.
-   Avoid placing lots of water since it is a known performance hog, and one that is not likely to be fixed in the foreseeable future.
-   For slopes shallower than 4:1, ramps are recommended; anything steeper should be done with stairs. A slope of exactly 4:1 can be done with either stairs or a ramp, depending on map styling and personal taste.
-   Place plenty of visual cues so that players can instantly identify where they are on the map; coloring rooms different colors makes them a lot easier to discern than everything covered in TrAK gray.
-   Take care to make the map feel like a part of a real continuum; ways to implement this include (but are not limited to) sound, landscape geometry, building geometry, skybox/cloudbox/cloudlayer/envlayer, fog, mapmodels, lighting, ambient, and sunlight.

**Other than that, level design is pretty easy!**
