### Graphical Settings

Red Eclipse has several tunable settings to allow flexible performance on varying levels of computer performance.

There are three main menus that deal with graphical settings: graphics, display, and resolution:

<img src="graphics.png" title="The graphics menu." alt="The graphics menu." width="960" height="520" />

The first is the graphics menu. It contains most of the effects that can be enabled or disabled. Let's go through them, one by one:

-   Shader detail: Disables many texture-based effects when disabled, including envmapping and specularity. It is recommended to leave this on unless the game is unplayable otherwise, since there generally is little to no performance penalty for enabling it.
-   Water: Reflection is a known performance hog, but it does make water appear much more realistic. Water refraction will make the water appear to have depth, and water envmapping will at least tint the water so that it somewhat approaches realism.
-   Waterfalls: Reflection without refraction looks ugly; the other way around is acceptable. Disabling both won't compromise the visuals nearly as much as with water.
-   Soft shadows: Affects the smoothness of player and actor shadows; has no effect on static shadows. Since you generally don't spend a ton of time staring at your own shadow, disabling this is advisable if you have performance problems.
-   Glare: Burns a lot of GPU time, but does improve visuals significantly. Many players disable this regardless of performance issues since it can be distracting.
-   Motion blur: Pretty useless, (slightly) blurs things that go fast, which is pretty much everything in RE. Most people disable this.
-   Grass: "Fade" refers to the radius at which the renderer fades out the grass to save computational power. Set this to whatever you prefer; be aware that grass heavy maps (though there are few) can be very strenuous on a GPU.
-   Dynamic lights: They are relatively rare, but are used to light places where lighting is not static (e.g. flickering lights). Disabling this may put you at a disadvantage in ability to see the map, but flickering effects may be annoying.
-   Soft particles: It's generally hard to pick up much detail in particles anyway, since most of them either move quickly or are too small to see clearly. Disabling this won't be a huge loss.
-   Glass: This applies to glass *material*, not alpha applied to standard geometry. It is recommended to enable and disable this along with shader detail, since it looks odd if the alpha effects are different than the glass material effects.
-   Decals: These are the impacts that are left by bullets hitting stuff. Set this to whatever you prefer; decals don't generally pose a performance problem in normal gameplay.
-   T-joints: This should be the absolute last thing to disable, since disabling it leaves artifacts at geometry corners.
-   Textures: May help performance on single-channel integrated graphics where the GPU is bandwidth-bound; otherwise, set this to high.
-   Models: This includes you. Disabling this will make your hands, as well as other players and mapmodels, ugly.

## User Content

User Content in Red Eclipse consists of all user configuration files, and any other content that they have downloaded or created. Specifically, this directory includes:

-   config.cfg, init.cfg, autoexec.cfg, localinit.cfg, servers.cfg
-   log.txt, servlog.txt
-   Custom content, such as user-made mapmodels, textures, or sounds
-   Saved maps
-   Downloaded maps
-   Files (.txt, .cfg) generated via the [/writevars](Variables#Game_Variables "wikilink") command

### Location

Each operating system has a designated directory (folder) to store user content. This is sometimes referred to as the Red Eclipse "home" directory. The location of this folder differs from OS to OS, and each location is outlined in the sections below.

The "home directory" location **can be changed**. See the [Client Command-line options](Client_Command_Line_Options#Filesystem_options "wikilink") page for more details.

#### Windows

The exact location varies on different versions of Windows, but the path can easily be found using [environment variables](http://en.wikipedia.org/wiki/Environment_variables#DOS.2C_OS.2F2_and_Windows_.28Command_Prompt.29), and can be used like this:

`%USERPROFILE%\My Documents\My Games\Red Eclipse`

##### XP

`C:\Documents and Settings\`<username>`\My Documents\My Games\Red Eclipse`

##### Vista/Win7

`C:\Users\`<username>`\My Documents\My Games\Red Eclipse`

##### Windows 8/Windows 10

The location varies depending on your system's configuration.

If your system is set up with OneDrive, check

`C:\Users\`<username>`\OneDrive\Documents\My Games\Red Eclipse`

Otherwise, check

`C:\Users\`<username>`\My Documents\My Games\Red Eclipse`

#### Linux

`~/.redeclipse`

#### Mac/OSX

`/Users/`<username>`/Library/Application Support/Red Eclipse`

### autoexec.cfg

This file, as it's name suggests, executes all commands listed in the file every time Red Eclipse is launched. It is used for numerous reasons including, but not limited to:

-   Executing arbitrary commands
-   Executing other scripts via \`**exec**\`
-   Creating user-defined command aliases
-   Keeping persistent user-defined settings
    -   Alternatively, this can be accomplished with the **setpersist** command.

This file does not exist by default and must be created.

### config.cfg

This is the main user configuration file. All game settings, options, keybinds and the like are stored here, and is updated automatically when Red Eclipse is closed. It is generally not necessary or recommended to edit this file; custom aliases/settings should go into **autoexec.cfg**. It may also be desirable to backup this file occasionally, as all custom binds and the like that are not stored in **autoexec.cfg** will be lost with the file in case of data corruption/deletion/etc.

### localinit.cfg

This file works in the same way that [servinit.cfg](https://sourceforge.net/apps/trac/redeclipse/browser/doc/examples/servinit.cfg) does, except it is used by the client's local server. In other words, when you play "offline practice".

### init.cfg

This file contains very specific and basic game settings that **should not be edited by hand**. Contains video and sound settings, among other important "under the hood" settings.

### servers.cfg

Contains a list of known servers that will be displayed in the server browser. You probably wont ever need to edit this by hand.

## How Custom Content is Loaded

When Red Eclipse is launched, the engine will first check for game files such as sounds, textures, config files, etc. in the "home" directory **and then** looks in the **data/** directory inside the installation directory. This allows custom content to be substituted by recreating the content structure found inside the **data/** directory.

For example, let's say you have a custom rifle zoom texture, and a custom firing sound for the rifle. If you wanted to use these instead of the defaults, simply place them in your Red Eclipse "home" folder exactly how they would be found inside the main **data/** directory.

<rehome>`/sounds/weapons/rifle/primary.ogg`
<rehome>`/textures/zoom.png`

Where *<rehome>* is the location of your Red Eclipse "home" directory. Notice how the directory structure is the same as that found in the **data/** directory. Now when you launch Red Eclipse, it will substitute the default files with the custom files inside your "home" directory. This way, the default content does not need to be overwritten, and all of your custom content stays with the rest of your configuration files.
