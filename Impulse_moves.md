This article aims to give an in-depth guide to the impulse system and movement techniques in Red Eclipse. For a compact summary of the basic moves and the default key bindings, please refer to the [Gameplay Controls](How_to_Play#Gameplay_Controls "wikilink").

## General

Unless otherwise specified, the following movement techniques are all impulse moves: They consume energy (as indicated by the impulse-meter shown in the [HUD (6)](How_to_Play#HUD "wikilink")) and they are also subject to the impulse count rule, as explained below.

### Impulse costs

Each impulse move depletes energy, which is recovered over time. The rate of this recovery depends on your current mode of movement: The more agile you are, the slower the regeneration. Therefore, crouching (default: left shift or C key) is the presumably quickest way to restore energy. However, some fearless runners claim that a stylish death right on a checkpoint can be even faster. If you run out of energy, you will be unable to execute impulse moves for a moment and you will be slowed down to walking speed. This is because running (impulse pace) is related to the impulse mechanics, albeit it does not consume any energy (per default).

### Impulse count

If you find yourself unable to execute an impulse move even though you have enough energy left, it is likely that you have reached the limit of the impulse count rule. It states that only a certain number of moves (default: six) can be performed in air before touching ground again. A typical situation where this rule applies is a long [wall-run](#Wall-run_.28tap.29 "wikilink") with some downwards motion.

### Impulse style

As will be explained later, only one successive impulse move can be executed in air, unless you hit a wall or a pusher. While this limitation is essential for the gameplay of Red Eclipse, it can be lifted with the impulsestyle variable, which can also disable the [impulse count](#Impulse_count "wikilink") rule.

### Impulse delay

Notwithstanding anything else, you can't use impulse moves of any kind if you've already used one over a recent, small window of time. (By default, the rate limit is 250ms, or ¼ of a second.) Impulse moves generally provide short-term speed boosts that fall off sharply as time goes on, so in order to conserve as much momentum as possible when chaining multiple moves in a row, and add to that momentum most effectively, it's best to get as close to that 250ms interval as possible every time. If you can't quite be that precise with your timing, it's often better to miss in the direction of slightly longer than 250 (which still allows you to perform your move with slightly less than optimal speed) instead of shorter than 250 (which causes the game to reject the move and possibly misinterpret your input as something else entirely, such as a simple jump that spoils all the extra momentum you had built up). Getting accustomed to the impulse delay window is most vital when performing multiple impulse slides; see below.

### Momentum and friction

Chaining impulse moves allows to build up momentum and gain exceptional movement speed. Up to some extent, this is compensated by friction (air- or groundcoast) which also governs air-control or grip. Higher friction (coast) means less control but better conservation of momentum. These and more environment variables like gravity can take special values on certain maps, and the grip can even differ for specific surfaces (vcoast).

### Weapon assisted movement

The kickpush when firing a weapon or the knockback (hitpush) when getting hit can significantly contribute to your [momentum](#Momentum_and_friction "wikilink"). This also applies to the shockwave of an explosion (wavepush), given that you can survive the detonation. The latter is referred as a rocket jump, but may need customized game variables to be useful. Note that the attractive force of the [plasma gun's](Weapons#Plasma "wikilink") secondary fire can also be used for trick jumps. In [time-trial](GameModes_and_Mutators "wikilink") games weapons are therefore often disabled using the [classic](GameModes_and_Mutators "wikilink") mutator.

## Basic moves

Basic moves are all you need to get started. Learning by doing is the best way to master them, but understanding the mechanics behind the moves can help you speed up the learning process.

### (ground) jump

The term jump is commonly used for various moves executed with the corresponding key (default: space). In a strict sense, however, jumps are only possible while either running, walking or standing on the ground. In contrast to similar moves, a jump does not consume any energy and can therefore be executed even while exhausted. The actual height of the jump depends on the current movement speed - the faster you move, the higher you will get.

### Impulse boost

The air dash or impulse boost is executed by pressing the jump key in air while holding a movement key (default: W, A, S, D or arrow keys). Doing so propels you exactly in the direction you are facing. It should be noted that this move can redirect your current [momentum](#Momentum_and_friction "wikilink") in the direction of the boost. Thus it allows to perform turns without losing speed, or even to convert falling speed into forwards or upwards [momentum](#Momentum_and_friction "wikilink").

### Double jump

Impulse boosts are frequently used to cover a wider distance with a [jump](#.28ground.29_jump "wikilink"), which works best by looking up in a 45° angle and pressing the jump key again as soon as downward motion sets in. This simple combo is sometimes referred as a double jump.

### Impulse jump

The impulse jump is often confused with the [impulse boost](#Impulse_boost "wikilink"), as both moves are performed with the jump key while in air. In contrast to the boost, an impulse jump requires to release the movement keys and always propels the player precisely upwards. This is very useful to slow down movement in the horizontal direction and to gain some extra height, for example if you want to land on a narrow platform.

### Wall-run

The wall-run is an essential move, as it greatly enhances your mobility and allows you to take advantage of your environment. It is executed with the special key (default: Q) while jumping at a wall and facing a direction parallel to its surface. Several related moves and combos are described in the next section. You can also [tap](Impulse_moves#Wall-run_.28tap.29 "wikilink") Q for better results.

### Wall-climb

If you jump and look either straight upwards or downwards, you can efficiently climb up a surface by holding the special key. When you find yourself bounce off the wall, try a steeper facing angle. While this move has a surprisingly wide vertical range, it renders you susceptible to enemy fire, as your trajectory is easily predictable.

## Standard moves

The following move set goes one step beyond the basics. Honing your skills allows you to manoeuvre much more quickly and to get past some obstacles in trial maps of moderate to advanced difficulty.

### Multi-boost

The simplest way to build up [momentum](#Momentum_and_friction "wikilink") is mashing the jump key while facing downwards slightly. This results in a zig-zag pattern consisting of [jumps](#.28ground.29_jump "wikilink") and [boosts](#Impulse_boost "wikilink"), which burns [energy](#Impulse_cost "wikilink") very rapidly. As it can be executed anywhere on ground, this move is useful to catch up with an enemy - or to prevent them from doing so.

### Vault

Vaulting allows you to boost over smaller obstacles - that are roughly below your center of mass - by simply holding the special key. This is highly convenient when you intend to jump on a very narrow platform, as you can vault while hitting the platforms edge. When timed right, the vault will propel you up in such a manner that you land exactly on the border of the platform.

### Impulse dash

If you double-tap a movement key while on the ground, you can execute an evasive manoeuvre, the impulse dash. This can be somewhat useful to build up [momentum](#Momentum_and_friction "wikilink") right before a jump when there is too little room for other moves. Performing a double-tap in air actually results in an [impulse boost](#Impulse_boost "wikilink") in the corresponding direction, so you can boost sidewards or backwards while keeping an eye on your target. Dash sidewards whilst moving forward to seamlessly circle an enemy.

### Push-boost

[Pushers](Entities#Types_of_Entities "wikilink") are elements of the environment that add, reset or redirect [momentum](#Momentum_and_friction "wikilink") as you touch them. They do not reset your [impulse count](#Impulse_count "wikilink"), but allow to perform an extra boost, just like after a [wall-run](#Wall-run_.28tap.29 "wikilink") or [-kick](#Wall-kick "wikilink"). Some pushers add plenty of [momentum](#Momentum_and_friction "wikilink"), which you may want to redirect to reach certain places. [Boosting](#Impulse_boost "wikilink") while or shortly after hitting a pusher can accomplish this. If proper timing gets difficult, button mashing may lead to success.

### Wall-run (tap)

A wall-run actually consists of several pushes that each consume some energy and contribute to the [impulse count](#Impulse_count "wikilink"). [Holding](#Wall-run_.28hold.29 "wikilink") the special key chains these pushes automatically, but not in an optimal manner. Thus one can release the special key between successive pushes, which allows to save energy and cover a wider distance without touching ground.

### Wall-jump

After a wall run, you can execute an [impulse boost](#Impulse_boost "wikilink") or [impulse jump](#Impulse_jump "wikilink") even if you did so before touching the wall. It is furthermore possible to jump off a wall while still performing the [wall-run](#Wall-run_.28tap.29 "wikilink"), which does not only help to build up [momentum](#Momentum_and_friction "wikilink"), but also allows to execute an additional [impulse boost](#Impulse_boost "wikilink") after the wall-jump. However, if you press the jump key when the [wall-run](#Wall-run_.28tap.29 "wikilink") has already ended, you will directly trigger an [impulse boost](#Impulse_boost "wikilink") and therefore be unable to chain another boost in air.

Note that if you start running on a wall too close to its edge, and in the direction of that edge, you might try to jump off while still attached to the wall, but the game can't accept your jump until the [impulse delay](#Impulse_delay "wikilink") expires. By that time, it's possible that your speed has carried you beyond the edge of the wall, so that your jump takes place in midair and counts as an impulse boost. If you need to take advantage of both a wall jump and a separate impulse boost to cover a long distance, make sure to give yourself enough space to run along the wall so you can actually do that while respecting impulse delay.

### Wall-kick

If you jump at a wall and press the special key while facing in the perpendicular direction, you will bounce away from the wall, which allows to redirect [momentum](#Momentum_and_friction "wikilink") and gain extra height. Your facing angle is important for this move: If it is perfectly orthogonal to the surface, you get pushed off the wall horizontally. Looking either up or down will gradually add an upwards component to your wall-kick. In this sense, the [wall-climb](#Wall-climb "wikilink") also consists of kicks.

### Kick-jump

It is possible to chain [impulse boosts](#Impulse_boost "wikilink") and [wall kicks](#Wall-kick "wikilink") alternately, until the [impulse count](#Impulse_count "wikilink") limit of six moves is reached. A typical application for this combo is to climb up steps in a ceiling that form an inverted stair.

## Advanced moves

The following list of movement techniques are of advanced difficulty. They allow you to discover shortcuts, get past trial maps of advanced to hard difficulty - or to have fun with stylish tricks during a death match.

### Slope-kick

Some slopes are too steep to jump off - landing on them will only cause you to slide down. However, you can still kick off the slope, just as you do on vertical surfaces with a [wall-kick](#Wall-kick "wikilink").

### Wall-dash

The wall-dash is a movement combo consisting of an [impulse boost](#Impulse_boost "wikilink"), [wall-run](#Wall-run_.28tap.29 "wikilink") and [wall-jump](#Wall-jump "wikilink"). All three moves need to be executed in quick succession to get the optimal result. This will build up considerable [momentum](#Momentum_and_friction "wikilink"), allowing you to cover much a wider distance than with a regular [wall-jump](#Wall-jump "wikilink").

### Air crouch

Some narrow passages with low ceilings can only be passed while crouching. When moving on ground, this will happen automatically, but if you want to jump into such a narrow passage, you will need to press the crouch key (default: Left shift or C).

### Crouch lock

On some systems, the use of the shift key for crouching can lead to conflicts with other keys. A typical symptom is that tapping shift while holding a movement key (running) renders you unable to jump - until you release the shift key, which then triggers one or multiple jump presses. If you experience this problem, try using another key to crouch. It will make moves like the [impulse launch](#Impulse_launch "wikilink") much more convenient and reliable.

### Power slide

There are three ways to perform a power slide:

-   Hold the crouch key and a movement key while landing on the ground.
-   Hold the crouch key and then do an [impulse dash](#Impulse_dash "wikilink") (double-tap a movement key).
-   Do an [impulse dash](#Impulse_dash "wikilink") and then hold the crouch key.

The slide is not only the heart of some advanced movement techniques, it also allows you to attack your foes by simply crashing into them.

### Impulse launch

Pressing jump while performing an [power slide](#Power_slide "wikilink") will propel you in the direction you are facing, much like an [impulse boost](#Impulse_boost "wikilink"), but potentially much more powerful. This will work best in the vertical direction and require rather precise timing. Although the impulse launch is executed while on ground, it does not allow you to perform a successive boost.

### Launch-climb

The most effective way to climb up a wall is to perform an [impulse launch](#Impulse_launch "wikilink"), hit the wall at full speed and then hold the special key for a [wall-climb](#Wall-climb "wikilink"). The actual height covered with this move depends strongly on your timing.

### Multi-slide

If you look downwards while performing an [impulse launch](#Impulse_launch "wikilink"), you gain considerable extra [momentum](#Momentum_and_friction "wikilink") without interrupting your slide. This move can be chained to reach impressive speeds with one single wide slide. However, if the downwards angle is too small, you will lose touch with the ground, which results in less acceleration and more [energy consumption](#Impulse_cost "wikilink").

### Super-launch

If you are able to perform a [multi-slide](#Multi-slide "wikilink"), why not convert that incredible speed into some upwards [momentum](#Momentum_and_friction "wikilink")? Right, finish your combo with an [impulse launch](#Impulse_launch "wikilink") and lift off like a rocket.

### Ladder-launch

[Ladder material](materials "wikilink") is a map element that enables movement in the vertical direction but prevents running (impulse pace) and boosting. However, if you [power slide](#Power_slide "wikilink") into ladder material, you can bypass this limitation and perform hilariously powerful chains of boosts.
