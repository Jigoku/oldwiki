This document was created by man2html and the online WikiConverter <http://labs.seapine.com/htmltowiki.cgi>

It refers to Red Eclipse as installed by the system-install target.

## NAME

redeclipse-server - script to launch the server for the Red Eclipse FPS game

## SYNOPSIS

\[ **-h**homedir \] \[ **-p**packagedir \] \[ **-o**sauerdir \] \[ **-g**logfile \]

\[ **-ss**{0..3} \] \[ **-sk**joinpass \] \[ **-sP**adminpass \] \[ **-sl**defaultmap \] \[ **-x**"command(s)" \]

\[ **-si**serverip \] \[ **-sp**serverport \] \[ **-sm**servermaster \] \[ **-sa**servermasterport \] \[ **-su**serveruprate \]

\[ **-ms**{0|1} \] \[ **-mi**masterip \] \[ **-mp**masterport \]

\[ **--help** \] \[ **-v**{0..4} \]

## DESCRIPTION

Red Eclipse is a single-player and multi-player first-person ego-shooter, built as a total conversion of Cube Engine 2, which lends itself toward a balanced gameplay, with a general theme of agility in a variety of environments.

**redeclipse-server** is a script which executes the **redeclipse-server** binary from the */usr/lib/games/redeclipse* directory.

The recommended way to change the settings of the server is to create and edit the files servexec.cfg and servinit.cfg files in your home directory. Examples are available in */usr/share/doc/redeclipse/examples/*

## OPTIONS

### Filesystem options

**-h***homedir*  
Sets your home directory to *homedir*. This is where servinit.cfg and servexec.cfg are read from, it defaults to *$HOME/.redeclipse/*.

  

**-p***packagedir*  
Includes the data files found in *packagedir*. Can be used for adding additional maps that may be distributed to clients. By default redeclipse-server only includes data files in the working directory */usr/share/games/redeclipse/data* and in the subdirecory *temp* of the home directory.

**-o***sauerdir*  
Sets the path to your Sauerbraten directory. If the Red Eclipse server can find your Sauerbraten directory, it will be able to load and distribute maps from it.

**-g***logfile*  
Output log to *logfile*. Path is set relative to *homedir*.

### Server [configuration](Server_Example_Configurations "wikilink") options

**-ss**{0..3}  
Sets server type. 0 for local only, 1 for private, 2 for public, 3 for dedicated. Defaults to 1.

**-sk***joinpass*  
Sets the join password to *joinpass*. Users must know the password before they can connect.

**-sP***adminpass*  
Sets the admin password to *adminpass*.

**-sc***maxclients*  
Sets the maximum number of clients to *maxclients*.

**-sl***defaultmap*  
Sets default map to *defaultmap*.

**-x***"command 1; command 2; ..."*  
Executes a list of commands once the Red Eclipse server has started up.

### Server connection options

**-si***serverip*  
Binds the server to the host address *serverip*. Only needed for machines with more than one interface.

**-sp***serverport*  
sets the server port to *serverport*.

**-sm***servermaster*  
Uses *servermaster* as the master server, defaults to play.redeclipse.net.

**-sa***servermasterport*  
Contacts the master server using port *servermasterport*, defaults to 28800.

**-su***serveruprate*  
Caps upstream rate to *serveruprate*. Once the cap is hit it will likely cause major connection glitching and disconnects. Use *maxclients* for bandwidth limiting instead.

### Master server options

**-ms**{0|1}  
Enables the server to act as a master server, defaults to 0.

**-mi**masterip  
Binds the master server to the host address *masterip*. Only needed for machines with more than one interface, defaults to *localhost*.

**-mp**masterport  
Binds the master server to the host port *masterport*, defaults to 28800.

### General options

**--help**  
Display this manpage

**-v**{0..4}  
Sets verbosity. This affects how much information is printed to the console. 0 is the least verbose, 4 is the most verbose.

## EXAMPLES

**redeclipse-server -p$HOME/mod/data -ss0 -slbath -sPpass**

  
Loads data from an additional directory, sets the server type to local (LAN), sets the default map to "bath" and sets the admin password to "pass"

**redeclipse-server -h$HOME/redeclipse-server\_configs/**

  
Reads and writes the configuration files to the specified directory instead of *$HOME/.redeclipse/*.

## AUTHORS

Red Eclipse's main developers are Quinton "quin" Reeves and Lee "eihrul" Salzman

This manual page was written by Martin Erik Werner &lt;<martinerikwerner@gmail.com>&gt;

## HISTORY

Red Eclipse was forked as a continuation of the game Bloodfrontier, which in turn was based on the Cube2 engine and the Sauerbraten game. Red Eclipse and Sauerbraten are now developed in parallel.
