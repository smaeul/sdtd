# 7 Days to Die XML configuration files

This repository contains both original and cleaned up version of the XML files
used to configure the game [7 Days to Die][official site]. It also contains some
minor mods and additional prefabs that I use locally on my multiplayer server.

[official site]: http://7daystodie.com/?home

## Branches in this repository

- `aX.Y-bZ`: Automatically cleaned up files for a specific version of the game.
  These files only have formatting changes and removed extraneous text. The XML
  as interpreted by the game should be exactly the same as the vanilla files.
  These are the files you want if you are doing research or creating a mod.
- `local-aX.Y-bZ`: The files as they existed on my server when it was running a
  specific version of the game. These branches are based on top of the
  respective `aX.Y-bZ` branch.
- `master`: The latest version of my customizations for the latest version of
  the game. This is exactly the same as `local-aX.Y-bZ` for the latest released
  build.
- `vanilla`: The latest version of the untouched XML files directly from Steam.
  The history of this branch will show you the changes made by the game
  developers over time.

## How to use these files

If you want to set up a server just like mine, use the master branch.

If you want to make your own modifications to these files, check out either the
latest `aX.Y-bZ` branch or the `vanilla` branch.

If you want to compare the differences between game versions, clone this
repository and run `git diff aA.B-bC..aX.Y-bZ`, replacing A/B/C and X/Y/Z with
the appropriate version numbers. It's important that you use two dots between
the branch names, so you compare the state of the files at the tips of the two
branches (and not from their fork point). Because the files in these branches
have consistent indentation and element ordering, the changes are really easy to
see and understand.

Unfortunately, GitHub does not provide a way of doing this kind of diff on their
web interface, so the best you can do without cloning is to view the history of
the `vanilla` branch.

## License of these files

The game developers encourage modding. My modifications are licensed under the
CC0. Don't think about it too hard.

## Other resources

- [7 Days Database](https://www.7daysdb.com/)
- [Default XMLs back to Alpha 11.6](http://7d2d.rocks/xml-defaults.php)
- ["7 Days To Mod" Modding Group](https://github.com/7daystomod)
- [GUI XML Editor](https://github.com/smaeul/7DaysToolbox) (old)
