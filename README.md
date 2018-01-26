```
text-editor

Jeffrey Lin, Arif Roktim
Period 5

A simple text editor written using curses.

--------------------------------------------------------------------------------

Requires the ncurses header files. On any system with apt:
# apt install libncurses5-dev libncursesw5-dev

--------------------------------------------------------------------------------

To build the project:
$ make

To debug Makefile statements:
$ V=[...] make [...]
or
$ make V=[...] [...]
The value of V does not matter.

After a debug session, you must clean the project before rebuilding:
$ make clean all

--------------------------------------------------------------------------------

To run the project:
$ make run

This presents the user with an empty buffer, in which they may write text.
Alternatively, you may specify a filename:
$ ./text-editor Makefile

--------------------------------------------------------------------------------

Not implemented:
You may not save the buffer. This is intentional.
You may not concatenate lines.
You may not write outside the boundaries of the screen.
You may not create new lines using the carriage return key.

--------------------------------------------------------------------------------

Not working:
Most of the code needed for networking support exists in the "bleeding" branch.
buffer.c:30 crashes while reallocating memory.
Status bar and command line don't work.
```

