To submit a [bug report](Readme#Get_Involved "wikilink") that concerns a crash to the Red Eclipse Team, it is helpful to have a backtrace.

## Windows (64 bit)

[You must download and install Code::Blocks for easiest building on Windows.](http://codeblocks.org)

### Setting up Code::Blocks

-   [Install TDM-GCC-64](https://sourceforge.net/projects/tdm-gcc/files/TDM-GCC%20Installer/tdm64-gcc-5.1.0-2.exe/download)
-   You may need to set the Code::Blocks compiler to TDM-GCC-64, open Code::Blocks and go to Settings -&gt; Compiler -&gt; Global Compiler Settings -&gt; Toolchain Executables. See the image example below for setting information.

### Compiling Red Eclipse

-   Open redeclipse.cbp in Code::Blocks as a project.
-   Select the debug build (redeclipse-amd64-dbg)
-   Press the Build button.

### Running Red Eclipse and Retrieving the Backtrace

-   Press the Debug/Continue button.
-   Red Eclipse will now start, attempt to crash it.
-   Once crashed, you will see the debugger near the bottom of the screen with a Command input. Write 'bt full' in that command input and press enter.
-   This will produce a backtrace, copy and paste this to an accessible place such as a crash report on the Red Eclipse forum or a paste service to be linked on IRC.

### Image Examples

<File:Win64dbg06.png%7CExample> compiler settings for TDM-GCC-64, paths may need changed depending on where you installed it. <File:Win64dbg01.png%7CSelecting> debug build. <File:Win64dbg02.png%7CPressing> the Build button. <File:Win64dbg03.png%7CPressing> the Debug button. <File:Win64dbg04.png%7CReady> to type 'bt full'. (Command input line near the bottom.)

## Linux

On Linux-based systems, you can use GDB to get a backtrace:

First you must compile with debug symbols:

``` bash
make -Csrc clean && CXXFLAGS=-ggdb3 make -Csrc install
```

Then run with GDB:

``` bash
gdb src/redeclipse_linux
```

Inside GDB, to start Red Eclipse:

``` text
run
```

Once Red Eclipse has crashed, GDB will catch this and present a prompt. At this prompt run:

``` text
bt full
```

This will produce a backtrace, copy and paste this to an accessible place such as a crash report on the Red Eclipse forum or a paste service to be linked on IRC.
