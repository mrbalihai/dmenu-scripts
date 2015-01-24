# dmenu-scripts
dmenu is a dynamic menu for X window. It enables searching of lots of menu items efficiently.
A collection of dmenu scripts to enable better window manager productivity.
I recommend using the xft patched version of dmenu because it looks much nicer with the smoother fonts.

dmenu : http://tools.suckless.org/dmenu/
dmenu-xft patch : http://tools.suckless.org/dmenu/patches/xft

## The Scripts
### dmenu-launch
Standard dmenu searching executables and running via exec

### dmenu-web
Open the default browser and begin a search using duckduckgo.
If the string is detected as a URL then it will open said URL.

The search engine can be changed by changing the 'SEARCH_ENGINE' variable at the top of the script, e.g.
`SEARCH_ENGINE="https://www.google.co.uk/#q="`

### Using the Scripts
I'm currently using Openbox in which you can edit `~/.config/openbox/rc.xml` and add hotkeys.
Here's what i use.

In the 'keyboard' section of rc.xml:

```
    <keybind key="C-A-w">
      <action name="Execute">
        <startupnotify>
          <enabled>true</enabled>
          <name>dmenu-web</name>
        </startupnotify>
        <command>~/dev/dmenu-scripts/dmenu-web</command>
      </action>
    </keybind>
    <keybind key="C-space">
      <action name="Execute">
        <startupnotify>
          <enabled>true</enabled>
          <name>dmenu-bind</name>
        </startupnotify>
        <command>~/dev/dmenu-scripts/dmenu-launch</command>
      </action>
    </keybind>
```
