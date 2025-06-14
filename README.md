# intellij-mnemonic-keymap-guide

* Install [Mnemonic Keymap](https://plugins.jetbrains.com/plugin/19094-mnemonic-keymap) plugin
* In `Files > Settings... > Keymap`
  * Choose Mnemonic Keymap on Windows or Mnemonic Keymap (macOS) on MacOS
  * Duplicate the keymap and rename it to something like `Mnemonic Keymap Custom` or `Mnemonic Keymap (macOS) Custom`
* Optionally but recommended, on MacOS, open `Apple logo > System Settings... > Keyboard > Keyboard Shortcuts... > Modifier Keys`
  and change the Control key to be Command key and vice versa.
  For people who work on both Windows and MacOS, this is very convenient.
  For example, the physical keyboard location of Command+C on MacOS is now the same as Ctrl+C on Windows.
* Refer to this [doc](https://github.com/dmimat/intellij-mnemonic-keymap) to check the base shortcuts of Mnemonic Keymap.
* Depend on each person, continue to customize shortcuts from the base Mnemonic Keymap.
  See below section for my personal recommended customizations.

# Recommended customizations

Best practices
* Adding new shortcuts instead of changing or removing default shortcuts of the Mnemonic Keymap plugin.
  So that less things to worry about when updating the plugin (ex. new shortcuts) or working on a new machine.
* 1st modifier key: Ctrl on Windows and Command/Cmd on MacOS
* 2nd modifier key
  * Shift: capitalization and symbols
  * Alt:
    * Mnemonic menu items, ex. `Alt+F` for **F**ile menu item (if **Enable mnemonics in menu** is checked)
    * Mnemonic UI buttons, ex. in commit window, `Alt+I` for comm**i**t button.
    * Enter a character by numeric code, ex. `Alt+0153` for the ™ symbol.
  * On MacOS, Alt is replaced with Option key.
    For example, `Alt+Enter` should be `Option+Enter` on MacOS.
    But if using just Option key, it mights replace the selection with a special char.
    In this case, use `Ctrl+Option` to replace Alt.
    For example, in commit window, use `Ctrl+Option+I` to replace `Alt+I`.
* Each double-chord shortcut should always have 2 versions.
  For example, when having `Ctrl+L,D`, we should have `Ctrl+L,Ctrl+D` too.
  `+` join keys for the same chord (pressing together). `,` separates chords.

| Action                          | Windows        | MacOS           | Notes                                                                |
| ------------------------------- | -------------- | --------------- | -------------------------------------------------------------------- |
| **D**uplicate Line or Selection | Ctrl+B,D       | Cmd+B,D         | Same as `Ctrl/Cmd+L,D`, which stands for Duplicate Line. `Ctrl+B,D` stands for Duplicate Block/Selection and only needs the left hand. |
| **D**elete Line                 | Shift+Delete   | Shift+Delete    | Need to remove this shortcut for Cut action                          |
| Paste as Plain Text             | Ctrl+Shift+V   | Cmd+Shift+V     | Need to use another shortcut for Paste Cell action in Jupyter plugin |
| **E**xtend Selection            | Ctrl+Shift+E   | Cmd+Shift+E     |                                                                      |
| **S**hrink Selection            | Ctrl+Shift+S   | Cmd+Shift+S     |                                                                      |
| **A**I **A**ssistant            | Ctrl+W,A       | Cmd+W,A         | Need to remove this shortcut for `Terminal > Delete Previous Word`, `Usage View Filtering > Show Write Access` |
| Windsurf                        |                |                 | https://github.com/xuanswe/intellij-mnemonic-keymap-guide/issues/3#issuecomment-2968810053 |
