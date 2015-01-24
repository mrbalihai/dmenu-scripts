# dmenu-scripts
dmenu is a dynamic menu for X window. It enables searching of lots of menu items efficiently.
A collection of dmenu scripts to enable better window manager productivity.
I recommend using the xft patched version of dmenu because it looks much nicer with the smoother fonts.

dmenu : http://tools.suckless.org/dmenu/
dmenu-xft patch : http://tools.suckless.org/dmenu/patches/xft

## dmenu-launch
Standard dmenu searching executables and running via exec

## dmenu-web
Open the default browser and begin a search using duckduckgo.
If the string is detected as a URL then it will open said URL.

The search engine can be changed by changing the 'SEARCH_ENGINE' variable at the top of the script, e.g.
`SEARCH_ENGINE="https://www.google.co.uk/#q="`
