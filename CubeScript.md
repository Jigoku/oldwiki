CubeScript is the scripting language of the [Cube 2 engine](http://cubeengine.com/). Such scripts can be entered via the [console](console "wikilink") or executed via files in the [user content directory](Game_Settings#User_Content "wikilink"). This allows to customize many aspects of the game (client) without the need to compile any sources.

## Applications

CubeScript can be used to

-   customize any of the existing in-game [menus](menus "wikilink") or create new [menus](menus "wikilink") from scratch,
-   enhance a custom map with [scripted events using triggers](Entity_Linking#Scriptable_Events "wikilink"),
-   write macros to automatize some actions or
-   load a set of game variables, such as weapon mods.

## Usage descriptions in the console

In the regular chat (or team chat) prompt, a leading forward slash (/) allows to execute commands via the console. The same can be done via the tilde (~) or forward slash (/) keys (per default).

The console supports tab-completion, which is very useful to cycle through the available [commands and variables](Vars_and_Commands_Tables "wikilink"). Just start typing and hit the *Tab* key to find matching commands or vars.

Usage instructions are available for many commands and game variables. These are displayed as a command is entered in the console, and they can also be looked up in the *variables* game menu, which offers advanced search options as well.

## Notation and containers

CubeScript uses prefix notation, which may seem strange at first: A command (or operator) is always followed by its arguments. For instance, *echo* will just print all of its arguments to the console.

`   /echo hello world`

Putting something in parenthesis will evaluate the result, so it can be used as an argument of another command. So for instance, calculating a term like

`   3*3 + 10`

looks a bit complicated:

`   /echo (+ (* 3 3) 10)`

Square bracket containers are used to form a block that will serve as a single argument. For example, the *newgui* command will define a new menu using two arguments: The menu name and content:

`   /newgui hello [guitext "hello world"]`

The menu can be shown any time later via *showgui*.

`   /showgui hello`

The two commands can be entered also on a single line using a semicolon. Note that there is only one slash at the beginning of the console input.

`   /newgui hello [guitext "hello world"]; showgui hello`

## Aliases and lookups

Aliases (variables) can be defined with the alias command or an assignment, which are equivalent as shown below.

`   /alias pi 3.14159`
`   /pi = 3.14159`

Note that game variables cannot be edited (redefined) this way. These are set by simply entering their name, followed by a new value as an argument, for example the player name.

` /playername frogger_afk`

The value of an alias can be looked up either via the $ token or (getalias), which again are equivalent

`   /echo (getalias pi)`
`   /echo $pi  `

$ tokens can be used recursively.

`   /varname = "pi"`
`   /echo $$varname`

There's a third way to look up an alias: The macro token @. However, this one is a bit different and more complicated to use. It will get the content of an alias (variable) before the beginning of the current \[\] block, and it can be chained to go back to a parent block.

`   /echo [@pi]`

Sounds complicated? It is, and in most cases not needed. For basic scripting, the $ token should be perfectly sufficient and save to use, while macros are convenient for inserting code snippets for advanced usage.

However, there's one important exception: For [menus](menus "wikilink") that use buttons in a loop, the button actions (or any *onchange* arguments) should use the @ token for a lookup of the control variable. Note that the $ token would return whatever is (or was!) assigned to that variable after the loop statement is completed.

` /newgui example [looplist i $weapname [guibutton $i [echo @i]]]`

On a single line, this example looks fairly complicated. Usually such scripts or [menus](menus "wikilink") are written in a text editor and saved as a *cfg* file.

## CubeScript files

If commands or variables are entered via the console, each line usually begins with a slash (/). In script files, however, there are no such leading slashes. The previous example (a test menu of weapon names) can be written as follows.

` newgui example [`
`     looplist i $weapname [`
`         guibutton $i [echo @i]`
`     ]`
` ]`
` showgui example`

This example script shows the use of square brackets to form blocks, which can be split on several lines. This allows to arrange the code for better readability, preferably with an indention of four spaces.

## Executing scripts

Scripts are typically saved as *cfg* files in the [user content directory](Game_Settings#User_Content "wikilink"). For example, the script in the file *myvars.cfg* can be executed using

`  /exec myvars.cfg`

Note that once you entered /exec, the *Tab* key can be used for auto-completion of filenames. Furthermore, scripts can be executed automatically using [autoexec.cfg](Game_Settings#autoexec.cfg "wikilink").

## Special string formatting

As a side note, there are some special tags to format strings with colours or icons, which can be fun to use, for instance in chat messages or in a /servermotd.

-   ^n - newline
-   ^" - a double quote sign
-   ^t - a (useless) tab
-   ^f - a format code as follows:
    -   ^f() - allows to insert a texture, for example "^f(textures/modes/race)hurry up!"
    -   ^f\[\] - use a hex code to colourize the text, for instance "^f\["$zappercolour"\]pzap!"
    -   ^fC - use the predefined colour C, or one of the below single letter colour codes:

**r**ed, **g**reen, **b**lue, **c**yan, **m**agenta, **y**ellow, **w**hite, gr**a**y, blac**k**, **v**iolet, **p**ink and brow**n**.

For most of these colours, a capital letter will result in a darker shade (except for K, V and N).

Furthermore, the letter z can be followed by two more colour tags to create flashing texts, for example

` "^fzyoBoOoM!"`

Flashing texts should be used with **caution**, as they can be very annoying - excessive use can get you muted.

Finally, the ^fs tag stores the current colour, such that it can be restored with a ^fS tag.

` "^frRed^fs^fbBlue^fSRed"`

## Example: Rainbow chat

Below is an example how the colour formats discussed above can be used in a chat script.

`   i = 0`
`   rainbowchat = [`
`       out = ""`
`       loop k $numargs [`
`           word = $(format "arg%1" (+ $k 1))`
`           loop j (stringlen $word) [`
`               out = (format "%1^fz%2%3" $out (substring "rygcbvmr" $i 2) (substring $word $j 1)) `
`               if (> $i 5) [i = 0 ] [i = (+ $i 1)]`
`           ]`
`           out = (format "%1 " $out)`
`       ]`
`       if (< (stringlen $out) 128) [`
`           say $out`
`       ] [`
`           echo (format "This message is %1 chars long - the usual limit is 127. Each letter takes up 5." (stringlen $out))`
`       ]`
`   ]`
`   `
`   setcomplete rainbowchat 1`
`   listcomplete rainbowchat [`
`       "BoOoM"`
`       "Good game!"`
`       "What the f*** was this?!?"`
`       "go for it!"`
`       "yeeeehaw!"`
`       "what a mess >_< "`
`   ]`

This defines a new command '/rainbowchat', which supports auto-completion - also for some predefined phrases. The following text is then parsed such that it is displayed in flashing rainbow colours. Since this inserts plenty of format tags, the overall length of the message is quite limited.

## CubeScript tutorials

For further reading, there are some detailed, external resources, such as the excellent tutorials by Hirato. For reference, here is also the corresponding documentation from sauerbraten.

-   <https://github.com/Hirato/lamiae/wiki/CubeScript>
-   <http://www.sandboxgamemaker.com/wiki/index.php?title=Cubescript>
-   <http://quadropolis.us/node/2336>
-   <http://sauerbraten.org/docs/config.html#cubescript>

These tutorials do not cover the gui elements used to create [menus](menus "wikilink") in Red Eclipse. For details, see the corresponding [article](menus "wikilink"), and most of all, have a look at the existing game [menus](menus "wikilink").
