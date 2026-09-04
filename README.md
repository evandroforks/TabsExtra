[![Unix Build Status][travis-image]][travis-link]
[![Package Control Downloads][pc-image]][pc-link]
![License][license-image]
# TabsExtra

Sublime Plugin with sticky tabs, more tab closing options, tab sorting, and tab access to cloning, deleting, renaming etc.

![Menu](docs/src/markdown/images/Menu.png)

# Features

- Adds `Close Tabs to the Left` for the current group.
- Adds `Close All Tabs` for the current group.
- Adds `Sticky Tabs` that allows a user select certain tabs that will not close when a tab close command is issued.
- Adds variants of the close commands to skip unsaved files, or to dismiss saved files with no prompt.
- Overrides the built-in tab commands and 'close' and 'close_all' commands to work with sticky tabs.
- Keep active window focus on delete, or default to the last active, left, or right tab (user configurable).
- Add open last tab, reveal in sidebar or finder, copy file path, save options, and revert.
- Adds tab sorting options (based loosely on @bizoo's [SortTabs](https://github.com/bizoo/SortTabs) plugin).
- Access clone, delete, rename, move, save, reveal, copy file path, revert, etc.


## Installation

### By Package Control

1. Download & Install **`Sublime Text 3`** (https://www.sublimetext.com/3)
1. Go to the menu **`Tools -> Install Package Control`**, then,
    wait few seconds until the installation finishes up
1. Now,
    Go to the menu **`Preferences -> Package Control`**
1. Type **`Add Channel`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
    input the following address and press <kbd>Enter</kbd>
    ```
    https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json
    ```
1. Go to the menu **`Tools -> Command Palette...
    (Ctrl+Shift+P)`**
1. Type **`Preferences:
    Package Control Settings – User`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
    find the following setting on your **`Package Control.sublime-settings`** file:
    ```js
    "channels":
    [
        "https://packagecontrol.io/channel_v3.json",
        "https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json",
    ],
    ```
1. And,
    change it to the following, i.e.,
    put the **`https://raw.githubusercontent...`** line as first:
    ```js
    "channels":
    [
        "https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json",
        "https://packagecontrol.io/channel_v3.json",
    ],
    ```
    * The **`https://raw.githubusercontent...`** line must to be added before the **`https://packagecontrol.io...`** one, otherwise,
      you will not install this forked version of the package,
      but the original available on the Package Control default channel **`https://packagecontrol.io...`**
    > [!WARNING]
    > Placing this custom channel before the default channel changes Package Control's resolution globally.
    > Packages from this channel with the same name will override versions from the default channel.
    >
    > You can review the channel contents here:
    > https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json
1. Now,
    go to the menu **`Preferences -> Package Control`**
1. Type **`Install Package`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
    search for **`TabsExtra`** and press <kbd>Enter</kbd>

See also:

1. [ITE - Integrated Toolset Environment](https://github.com/evandrocoan/ITE)
1. [Package control docs](https://packagecontrol.io/docs/usage) for details.


# Documentation

http://facelessuser.github.io/TabsExtra/

# License

TabsExtra is released under the MIT license.

Copyright (c) 2014 - 2017 Isaac Muse <isaacmuse@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

[travis-image]: https://img.shields.io/travis/facelessuser/TabsExtra/master.svg
[travis-link]: https://travis-ci.org/facelessuser/TabsExtra
[pc-image]: https://img.shields.io/packagecontrol/dt/TabsExtra.svg
[pc-link]: https://packagecontrol.io/packages/TabsExtra
[license-image]: https://img.shields.io/badge/license-MIT-blue.svg
