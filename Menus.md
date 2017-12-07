**Important note:** The information in this article is valid for the current release version, but will soon be outdated. For the upcoming menu system, see [New ui](New_ui "wikilink").

All menus or guis of Red Eclipse are written in [CubeScript](CubeScript "wikilink") using a set of gui commands. This means the menus can be simply modified with a text editor, without the need to compile any source code. The existing menus are therefore conveniently customized - and they also provide a large set of examples for creating your own custom menus. Such menus could be used in a campaign-like map, or for example to execute administrative commands.

## Preface

### Accessing the in-game menus

The game-menus are found in a subdirectory of the Red Eclipse install directory:

` /config/menus/`

The corresponding link to the development version on github is [here](https://github.com/red-eclipse/base/tree/master/config/menus).

When customizing the in-game menus, it is highly recommended to leave the files unmodified in the install directory, and work on a copy in the [user content directory](Game_Settings#User_Content "wikilink"). In this case, the in-game menus can be overriden by executing the modified script

` exec mymenu.cfg`

### A minimalistic example

The following script will define and display a menu with just a title and one text line.

` newgui hello [`
`     guitext "hello world"`
` ]`
` showgui hello`

### A test alias

If you are familiar with the use of aliases and [CubeScript](CubeScript "wikilink"), you can quickly test and preview gui commands via the [console](console "wikilink"). For example, the following alias can be used:

` /testgui = [ newgui test [ @arg1 ] ; showgui test ]`

To reproduce the minimalistic example above, this alias can be used as follows:

` /testgui [guitext "hello world"]`

This may seem fairly complicated, but it can be convenient to read the [usage descriptions](CubeScript#Usage_descriptions_in_the_console "wikilink") and quickly check how the commands work.

### Use of gui commands

The following sections describe many of the available gui elements and commands, which are usually not covered in external [CubeScript](CubeScript "wikilink") tutorials. These commands typically have some optional arguments, which are shown in \[brackets\] and can be rather complicated to use.

If a command is entered in the [console](console "wikilink"), usage instructions are indicated in many cases. This also holds true for many gui commands, and roughly corresponds to the following descriptions.

The ordering of a command's arguments matters. This means that, for instance, if you want to specify the colour (third argument) of a guibutton, a texture (second argument) must be given as well:

` guitext "just a test line" "" 0xffff00 `

In this case, the empty texture string "" simply means that no icon is shown next to the button.

## creation and display of menus

### guiheader

sets the header title of the menu, replacing the first argument of newgui in the title bar.

usage: guiheader *value*

### guistayopen

Usually, clicking a button or image to trigger an action will close the menu.

This rule does not apply to buttons or images in a guistayopen block.

usage: guistayopen *content*

### guitab

creates a new tab for the current menu. Note: The first tab of each menu is already impied by newgui.

usage: guitab *name*

### guicount

Returns the number of menus in the current gui stack.

## basic gui elements

### guitext

creates a text element;

-   *text* can be a raw string or a variable,

<!-- -->

-   \[*icon*\] is the path to an image, example: textures/bomb,

<!-- -->

-   \[*colour*\] is a hexadecimal colour code, example: 0xFF0000,

<!-- -->

-   \[*iconcolour*\] acts on the *icon* just like *colour* acts on the *text*,

<!-- -->

-   \[*wrap*\] specifies a width limit, which allows the text to expand over several lines

usage: guitext *text* \[*icon*\] \[*colour*\] \[*iconcolour*\] \[*wrap*\]

### guibutton

creates a text button;

-   *name* refers to the button's variable name,

<!-- -->

-   *action* defines what the button does,

<!-- -->

-   \[*alt-act*\] defines what the button does when right-clicked,

<!-- -->

-   \[*icon*\] is the path to an image, example: textures/bomb,

<!-- -->

-   \[*colour*\] is a hexadecimal colour code, example: 0xFF0000

usage: guibutton *name* *action* \[*alt-act*\] \[*icon*\] \[*colour*\]

### guiimage

creates a clickable image;

-   *path* is the path to an image, example: textures/bomb,

<!-- -->

-   \[*action*\] defines what clicking the image does,

<!-- -->

-   \[*scale*\] defines the scale of the image,

<!-- -->

-   \[*overlaid*\] whether or not the image is overlaid with guioverlaytex (true/false),

<!-- -->

-   \[*alt-path*\] alternate image to use if *path* cannot be loaded,

<!-- -->

-   \[*alt-act*\] defines what the image does when right clicked,

<!-- -->

-   \[*colour*\] is a hexadecimal colour code - useful to colorize icons, e.g. for weapons or teams

usage: guiimage *path* \[*action*\] \[*scale*\] \[*overlaid*\] \[*alt-path*\] \[*alt-act*\] \[*colour*\]

### guicheckbox

creates a checkbox;

-   *name* a text string shown to the right of the checkbox,

<!-- -->

-   *variable* refers to the alias/var that the checkbox controls,

<!-- -->

-   \[*on*\] is the value given to *variable* when the checkbox is on, and vice-versa for \[*off*\], if these are not specified, 1/0 is assumed,

<!-- -->

-   \[*onchange*\] is the action taken whenever the checkbox is toggled,

<!-- -->

-   \[*colour*\] is a hexadecimal colour code, example: 0xFF0000

usage: guicheckbox *name* *var* \[*on*\] \[*off*\] \[*onchange*\] \[*colour*\]

### guiradio

creates a radio button;

-   *name* a text string shown to the right of the radio button,

<!-- -->

-   *var* refers to the alias/var that the radio button controls,

<!-- -->

-   *value* is the value given to *var* when selected,

<!-- -->

-   \[*onchange*\] is the action taken whenever the button is toggled,

<!-- -->

-   \[*colour*\] is a hexadecimal colour code, example: 0xFF0000

usage: guiradio *name* *var* *value* \[*onchange*\] \[*colour*\]

## gui layout elements

### guilist

adds *content* to a list. Guilists can be nested to arrange gui elements horizontally and vertically.

This also allows to structure the layout in order to use guibars, guisliders and coloured guibackgrounds.

usage: guilist *content*

### guibody

allows a list of gui elements to act like a single button;

-   *content* is a block of code inside an implied guilist,

<!-- -->

-   *action* is the action taken when clicking any element of *content*

<!-- -->

-   \[*alt-act*\] allows to define a different right-click action,

<!-- -->

-   \[*onhover*\] is executed when the mouse moves over the boundary of the guibody - useful for guitooltip

usage: guibody *content* *action* \[*alt-act*\] \[*onhover*\]

### guispring

adds weight to a menu for pushing elements more/less to one side;

example: guilist \[ guispring ; guitext centered; guispring \]

usage: guispring \[*value*\]

### guistrut

adds spacing to a menu;

if \[*bool*\] is 1, it wraps the guistrut in a guilist (adds spacing in the alternate direction),

guistrut 5 1 is the same as guilist \[ guistrut 5 \]

usage: guistrut *amount* \[*bool*\]

### guibar

draws either a vertical or a horizontal line, depending on the nesting of guilist

### guifont

sets the text font to be used in a block;

-   *font* is a keyword, e.g. emphasis or small

<!-- -->

-   *block* is a block of gui elements for which *font* is used

example: newgui font-preview \[loopfiles i config/fonts cfg \[guifont $i \[guitext $i\]\]\]

note: This will preview all of the available *font* options.

usage: guifont *font* *block*

### guibackground

creates a colored background for the current guilist;

-   *colour* is in hexadecimal, example: 0xFF0000,

<!-- -->

-   \[*blend*\] is the opacity of the colour, ranges from 0 (invisible) to 1 (opaque),

<!-- -->

-   \[*bordercolour*\] is the colour of the border,

<!-- -->

-   \[*borderblend*\] is the opacity of the border,

<!-- -->

-   \[*border*\] determines if the border is drawn (0 or 1),

<!-- -->

-   \[*levels*\] specifies how many guilist levels to go back

usage: guibackground *colour* \[*blend*\] \[*bordercolour*\] \[*borderblend*\] \[*border*\] \[*levels*\]

### guifill

creates a coloured background for the current guilist, but without the skin settings of guibackground.

This implies sharp corners, no borders and a blend value of 0.5;

-   *colour* is in hexadecimal, example: 0xFF0000,

<!-- -->

-   \[*levels*\] specifies how many guilist levels to go back

usage: guifill *colour* \[*levels*\]

## advanced gui elements

### guifield

creates a text field;

-   *var* is the variable the guifield controls,

<!-- -->

-   *maxlength* is the width in characters, negative values allow the field to expand downward,

<!-- -->

-   \[*onchange*\] is the action taken when the value changes,

<!-- -->

-   \[*colour*\] is a hex colour, e.g. 0xFF0000,

<!-- -->

-   \[*focus*\] (1) will keep the input field in focus,

<!-- -->

-   \[*parent*\] allows to pass the input,

<!-- -->

-   \[*height*\] is the number of lines to show with a scroll bar,

<!-- -->

-   \[*promt*\] is a text shown when *var* is empty,

<!-- -->

-   \[*immediate*\] (1) updates *var* already while typing.

usage: guifield *var* *maxlength* \[*onchange*\] \[*colour*\] \[*focus*\] \[*parent*\] \[*height*\] \[*promt*\] \[*immediate*\]

### guieditor

creates a guifield with content from a text file;

-   *name* is a filename,

<!-- -->

-   \[*maxlength*\] is the width of the field, negative values imply text wrap,

<!-- -->

-   \[*height*\] is the number of lines shown with a scroll bar,

<!-- -->

-   \[*mode*\] (4) implies read-only,

<!-- -->

-   \[*colour*\] is a hex code for the entire editor,

<!-- -->

-   \[*focus*\] (1) keeps the editor field in focus

<!-- -->

-   \[*parent*\] allows to pass input,

<!-- -->

-   \[*str*\] allows to do a textinit using *name*,

<!-- -->

-   \[*prompt*\] is shown when the field is empty.

usage: guieditor *name* \[*maxlength*\] \[*height*\] \[*mode*\] \[*colour*\] \[*focus*\] \[*parent*\] \[*str*\] \[*prompt*\]

### guikeyfield

creates a key field (each key being a separate element);

-   *var* refers to the alias/variable the guikeyfield controls,

<!-- -->

-   *maxlength* defines the maximum number of characters/length of the field, negative values allow the field to expand downward as needed,

<!-- -->

-   \[*onchangge*\] is the action taken when the guikeyfield value changes,

<!-- -->

-   \[*colour*\] is a hexadecimal colour code example: 0xFF0000

usage: guikeyfield *var* *maxlength* \[*onchange*\] \[*colour*\]

### guibitfield

creates a checkbox for the bitwise and of *var* and *bit*;

-   *name* a text string shown to the right of the checkbox,

<!-- -->

-   *variable* refers to an alias/var that holds bitwise information,

<!-- -->

-   *bit* is the bit of *var* that the checkbox controls, given as a power of 2,

<!-- -->

-   \[*onchange*\] is the action taken whenever the checkbox is toggled,

<!-- -->

-   \[*colour*\] is a hexadecimal colour code, example: 0xFF0000.

example: guibitfield allow votes for race games modelockfilter $modebitrace

usage: guibitfield *name* *var* *bit* \[*onchange*\] \[*colour*\]

### guislider

creates a slider, depending on the use of guilist;

-   *var* is an integer that the slider controls,

<!-- -->

-   *min* and *max* give the valid range for *var*,

<!-- -->

-   \[*onchange*\] is the action taken when the slider is moved,

<!-- -->

-   \[*reverse*\] (1) flips the slider,

<!-- -->

-   \[*scroll*\] (1) enables scrolling also on the parent guilist,

<!-- -->

-   \[*colour*\] is a hex colour (hover text),

<!-- -->

-   \[*style*\] (1) draws a bar instead of a point,

<!-- -->

-   \[*slidercolour*\] is a hex colour (bar/point).

example: guislider raceweapon 0 11

see also: guinameslider, guilistslider

usage: guislider *var* *min* *max* \[*onchange*\] \[*reverse*\] \[*scroll*\] \[*colour*\] \[*style*\] \[*slidercolour*\]

### guilistslider

creates a slider, depending on the use of guilist;

-   *var* is an integer that the slider controls,

<!-- -->

-   *list* holds the values for *var*,

<!-- -->

-   \[*onchange*\] is the action taken when the slider is moved,

<!-- -->

-   \[*reverse*\] (1) flips the slider,

<!-- -->

-   \[*scroll*\] (1) enables scrolling also on the parent guilist,

<!-- -->

-   \[*colour*\] is a hex colour (hover text),

<!-- -->

-   \[*style*\] (1) draws a bar instead of a point,

<!-- -->

-   \[*slidercolour*\] is a hex colour (bar/point).

example: guilistslider raceweapon \[0 1 2 3 4 5 6 7 8 9 10 11\]

see also: guinameslider

usage: guilistslider *var* *list* \[*onchange*\] \[*reverse*\] \[*scroll*\] \[*colour*\] \[*style*\] \[*slidercolour*\]

### guinameslider

creates a slider, depending on the use of guilist;

-   *var* is an integer that the slider controls,

<!-- -->

-   *names* is a list of hover texts shown for each value,

<!-- -->

-   *list* is a list of valid values for *var*,

<!-- -->

-   \[*onchange*\] is the action taken when the slider is moved,

<!-- -->

-   \[*reverse*\] (1) flips the slider,

<!-- -->

-   \[*scroll*\] (1) enables scrolling also on the parent guilist,

<!-- -->

-   \[*colour*\] is a hex colour (hover text),

<!-- -->

-   \[*style*\] (1) draws a bar instead of a point,

<!-- -->

-   \[*slidercolour*\] is a hex colour.

example: guinameslider raceweapon $weapname \[0 1 2 3 4 5 6 7 8 9 10 11\]

usage: guinameslider *var* *names* \[*list*\] \[*onchange*\] \[*reverse*\] \[*scroll*\] \[*colour*\] \[*style*\] \[*slidercolour*\]

### guimodelpreview

shows a preview of a mapmodel

-   *model* is a subdirectory of data/models

<!-- -->

-   \[*animspec*\] is the name of an associated animation,

<!-- -->

-   \[*action*\] allows to use the preview as a button,

<!-- -->

-   \[*scale*\] is the preview image size,

<!-- -->

-   \[*overlaid*\] (1) draws a frame (guioverlaytex),

<!-- -->

-   \[*size*\] is a scaling or zoom factor,

<!-- -->

-   \[*blend*\] is for opacity,

<!-- -->

-   \[*alt-act*\] defines an action for right-clicking

usage: guimodelpreview *model* \[*animspec*\] \[*action*\] \[*scale*\] \[*overlaid*\] \[*size*\] \[*blend*\] \[*altact*\]

### guiplayerpreview

shows a preview of a player model;

-   \[*model*\] is 0 (male) or 1 (female),

<!-- -->

-   \[*colour*\] is the player colour,

<!-- -->

-   \[*team*\] is the team index (0-4),

<!-- -->

-   \[*weap*\] is a weapon id (0-11),

<!-- -->

-   \[*vanity*\] is a list of vanity item names,

<!-- -->

-   \[*action*\] allows to use the preview as a button,

<!-- -->

-   \[*scale*\] is the preview image size,

<!-- -->

-   \[*overlaid*\] (1) draws a frame (guioverlaytex),

<!-- -->

-   \[*size*\] is a scaling or zoom factor,

<!-- -->

-   \[*blend*\] is for opacity,

<!-- -->

-   \[*alt-act*\] defines an action for right-clicking

usage: guiplayerpreview *model* *colour* *team* *weap* *vanity* \[*action*\] \[*scale*\] \[*overlaid*\] \[*size*\] \[*blend*\] \[*altact*\]

### guiprogress

draws an animated progress icon, as shown when loading a map;

-   *value* is converted to a percentage and used as an overlay text,

<!-- -->

-   \[*size*\] is the image size for the progress icon

usage: guiprogress *value* \[*size*\]

### guislice

creates a slice (pie-chart) of an image with overlaid text;

-   \[*path*\] is the path to an image, example: textures/bomb ,

<!-- -->

-   \[*action*\] is executed when clicking the image,

<!-- -->

-   \[*scale*\] is the size of the image,

<!-- -->

-   \[*start*\] and \[*end*\] give the range of the slice. For a full rotation, use 0 1,

<!-- -->

-   \[*text*\] is an overlay text,

<!-- -->

-   \[*altpath*\] is used when *path* cannot be loaded,

<!-- -->

-   \[*altact*\] allows to specify a different right-click action

usage: guislice \[*path*\] \[*action*\] \[*scale*\] \[*start*\] \[*end*\] \[*text*\] \[*altpath*\] \[*altact*\]

## hover effects

### guinohitfx

Hover effects are disabled for all buttons or images in a guinohitfx block.

This is useful for images that do not act as buttons.

usage: guinohitfx *content*

### guitooltip

creates a text box attached to the mouse pointer;

-   *text* is the hover text,

<!-- -->

-   \[*width*\] adjusts the width of the box,

example: if (=s $guirolloveraction disconnect) \[guitooltip leave the current game (server)\]

usage: guitooltip *text* \[*width*\]

### guirollovername

Returns the text label or image path of the gui element at the current mouse position.

### guirolloveraction

Returns the *action* of a button or image or the *var* of a checkbox or radio at the current mouse position.

### guirollovertype

Returns the type of the gui element at the current mouse position, e.g. text, image or checkbox.

## Glue functions

A collection of aliases for some gui commands is found in the file

` /config/menus/glue.cfg`

For example, this allows to create centered text (using springs) or boxed frames in menu. These aliases are also used in many of the in-game menus.
