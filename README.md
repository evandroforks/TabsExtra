TabsExtra
=========

Sublime Plugin with sticky tabs and more tab closing options.  ST3 is the only **officially** supported platform.

# Features

- Adds `Close Tabs to the Left`
- Adds `Close All Tabs`
- Adds `Sticky Tabs` that allows a user select certain tabs and close just those, or close the inverse of those
- Adds `Close Sticky Tabs`
- Adds `Close Non-Sticky Tabs`
- Overrides the built-in tab commands to work with sticky tabs (ST3 only)

# Sticky Tab Settings
You can make non `Sticky` commands not close `Sticky` tabs by enabling the following setting:

```javascript
    "all_commands_respect_sticky": false
```

By default, after any `Close` command is run, all `Sticky` tab properties are removed.  You can make a tab's `Stickiness` persist by enabling the following setting:

```javascript
    "persistent_sticky": false,
```

# Tab Context Menu Options
By default, the commands won't be grouped together because of the way Sublime Text menus are managed.  But you can optionally install a menu that overrides the Default Package's tab context menu for sane grouping of the commands.

# ST2 Support?
ST2 support is not officially complete.  For best functionality, it is recommended to install the override menu for the Default tab context menu.
