# Iterm
Iterm is essentially a better terminal.  If you want to customize the
look or feel in some way, try

Command-, (command comma)

to bring up the full-screen terminal window, do

Command-esc (command escape)

# Command line
[this](https://explainshell.com/) website is a godsend.

A few quick things:

+ ```$ mkdir <dirname>``` makes a directory called <dirname>
+ ```$ mv <filename> <path/to/new/filename>``` moves filename to the
directory or name specified by <path/to/new/filename>
+ ```$ command_1 && command_2``` executes command\_1 then command\_2

# Emacs tutorial!

For a more complete and better-written document,
try [this](https://www.emacswiki.org/emacs/EmacsNewbieKeyReference)

## How to read commands

+ ```C-<key>``` means ```control + <key>```
+ ```M-<key>``` means ```alt + <key>```

## General comands

### Prefix keys

Prefix keys are key sequences that tell emacs how to interpret the
keys (or sequences of keys) that follow it.

+ C-x is a prefix key for feeding "global" commands to emacs. Things
  like saving files, quitting emacs, or other things that aren't
  dependent on the current mode will likely be some form of C-x command.
+ C-c is for commands that are specific to the current mode. E.g., in
  latex-mode, C-c C-c opens the command menu for compiling/viewing a
  latex document.

# tmux
See [tmux cheat sheet](https://gist.github.com/MohamedAlaa/2961058)

tmux is basically a way of getting tabs in your terminal.  But, it
also keeps a record of the state of your terminal.  If you have an
unexpected crash, you can restore your session by doing

```$ tmux attach -t <session-number>```

Where <session-number> is the boxed number in the lower left corner of
the screen.  If you aren't sure what sessions you had open, you can do

```$ tmux ls ```

which will list all the tmux sessions you had open, along with some
brief information about them.

## prefix keys

You need to feed a command to the terminal to tell it that you're
doing a tmux command instead of a regular command.  To do this, use a
~.  The web tutorial will tell you you need C-b.  C-b has been rebound
to ~.

+ ~-c makes a new pane
+ ~-x kills the current pane
+ ~-, renames the current pane
+ ~-<number> takes you to the given window
+ ~-" splits the pane horizontally
+ ~-% splits the pane vertically
+ ~-l goes to the previous pane
+ ~-n goes to the next pane
