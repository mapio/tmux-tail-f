# tmux tail -f

This tool allows to tail a set of files in a multi-pane
[tmux](http://tmux.sourceforge.net/) window.

```
$ tmux-tail-f -H
Usage: tmux-tail-f [OPTION]... [FILE]...
Tail the FILEs in a tmux window, one per pane.

Optional arguments:
  -v     use the 'even-vertical' layout (default).
  -h     use the 'even-horizontal' layout.
  -t     use the 'tiled' layout.
  -H     print this help.
```
