## Vote filtering

If you wish to limit voting on your server to only certain [modes or mutators](GameModes_and_Mutators "wikilink") you will need to

-   Take all the the **bit shifted** values for the [modes](#Modes "wikilink")/[mutators](#Mutators "wikilink") you want to allow
-   Add them up
-   Use this sum value for the **sv\_modelockfilter**/**sv\_mutslockfilter** variable

For example, to lock voting to only deathmatch and bomber-ball you need 4 + 32 = 36

`sv_modelockfilter 36`

This will also lock the voting to only the allowed maps for those modes.

As of Red Eclipse 1.3 (Galactic Edition), there are now "idx vars" that represent each bit-shifted value for each mode and mutator. These vars can be easily added when changing settings that involve these filters. For example:

`sv_modelockfilter (+ $modebitdeathmatch $modebitcapture)`

Would limit the server to deathmatch and capture the flag

To allow the admin to override the filter, set

`sv_modelock 3`

It is not possible to disable voting for mutators completely, but you can get close by using

`sv_mutslockfilter 65536`

which will only keep the third mode variation mutator (ctf-protect) enabled.

## Server Rotation Filtering

If you wish to filter the server rotation (without blocking rotation completely) use the **sv\_rotatemodefilter**/**sv\_rotatemutsfilter** variables

For example

`sv_rotatemodefilter 36`

## Filter Values

### Modes

| Number | Bit shifted | Mode             | idxvar            |
|--------|-------------|------------------|-------------------|
| 0      | 1           | Demo             | modebitdemo       |
| 1      | 2           | Editing          | modebitediting    |
| 2      | 4           | Deathmatch       | modebitdeathmatch |
| 3      | 8           | Capture the Flag | modebitcapture    |
| 4      | 16          | Defend the Flag  | modebitdefend     |
| 5      | 32          | Bomber-ball      | modebitbomber     |
| 6      | 64          | Race             | modebitrace       |
||

### Mutators

| Number | Bit shifted | Mutator                                                                       | idxvar           |
|--------|-------------|-------------------------------------------------------------------------------|------------------|
| 0      | 1           | Multi                                                                         | mutsbitmulti     |
| 1      | 2           | Free-for-all                                                                  | mutsbitffa       |
| 2      | 4           | Co-op                                                                         | mutsbitcoop      |
| 3      | 8           | Instagib                                                                      | mutsbitinsta     |
| 4      | 16          | Medieval                                                                      | mutsbitmedieval  |
| 5      | 32          | Kaboom                                                                        | mutsbitkaboom    |
| 6      | 64          | Duel                                                                          | mutsbitduel      |
| 7      | 128         | Survivor                                                                      | mutsbitsurvivor  |
| 8      | 256         | Classic                                                                       | mutsbitclassic   |
| 9      | 512         | Onslaught                                                                     | mutsbitonslaught |
| 10     | 1024        | Freestyle                                                                     | mutsbitfreestyle |
| 11     | 2048        | Vampire                                                                       | mutsbitvampire   |
| 12     | 4096        | Resize                                                                        | mutsbitresize    |
| 13     | 8192        | Hard                                                                          | mutsbithard      |
| 14     | 16384       | Basic                                                                         | mutsbitbasic     |
| 15     | 32768       | First mode variation (ctf-quick, dtf-quick, bomber-hold, gauntlet-timed)      | mutsbitgsp1      |
| 16     | 65536       | Second mode variation (ctf-defend, dtf-king, bomber-touchdown, gauntlet-hard) | mutsbitgsp2      |
| 17     | 131072      | Third mode variation (ctf-protect)                                            | mutsbitgsp3      |
||

## How the Filter Values Work

Filters are simply created using bitwise OR (numbers are bit shifted first):

Example: 2 (Deathmatch) + 5 (Bomber Ball) = (1&lt;&lt;2) + (1&lt;&lt;5) = 4 + 32 = 36

`00000100 +`
`00100000 =`
`00100100 (binary) = 36 (decimal)`
