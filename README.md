# tmux tail -f

This tool allows to tail a set of files in a multi-pane
[tmux](http://tmux.sourceforge.net/) window.

```
$ tmux-tail-f -H
Usage: tmux-tail-f [OPTION]... [FILE]...
Tails the FILEs in a tmux window, one per pane; hitting `^C` in
any one of the panes will terminate all the tail commands and
kill the tmux session.  Uses the `-F` option instead of `-f`,
which keeps trying to open a file if it is inaccessible.

Optional arguments:
  -v     use the 'even-vertical' layout (default).
  -h     use the 'even-horizontal' layout.
  -t     use the 'tiled' layout.
  -H     print this help.
  -U     update this script to the latest version.
```

For example

```
tmux-tail-f -h /var/log/httpd/{access,error}_log
```

will show the Apache logs in a tmux window split in two panes.

This tool is heavily inspired by [mtmux](https://github.com/wbond/mtmux).

![Analytics](https://ga-beacon.appspot.com/UA-377250-20/tmux-tail-f?pixel)
