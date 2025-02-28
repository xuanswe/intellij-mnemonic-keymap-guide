# intellij-mnemonic-keymap-guide

* Install [Mnemonic Keymap](https://plugins.jetbrains.com/plugin/19094-mnemonic-keymap) plugin
* In `Files > Settings... > Keymap`
  * Choose Mnemonic Keymap on Windows or Mnemonic Keymap (macOS) on MacOS
  * Duplicate the keymap and rename it to something like `Mnemonic Keymap Custom` or `Mnemonic Keymap (macOS) Custom`
* Optionally, on MacOS, open `Apple logo > System Settings... > Keyboard > Keyboard Shortcuts... > Modifier Keys`
  and change the Control key to be Command key and vice versa.
  For people who work on both Windows and MacOS, this is very convenient.
  For example, the physical keyboard location of Command+C on MacOS is now the same as Ctrl+C on Windows.
* Refer to this [doc](https://github.com/dmimat/intellij-mnemonic-keymap) to check the shortcuts
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
    * Mnemonic menu items, ex. Alt+F for **F**ile menu item (if **Enable mnemonics in menu** is checked)
    * Mnemonic UI buttons, ex. in commit window, `Alt+I` for comm**i**t button.
    * Enter a character by numeric code, ex. `Alt+0153` for the ™ symbol.

| Action                          | Windows        | MacOS           | Notes                                                             |
| ------------------------------- | -------------- | --------------- | ----------------------------------------------------------------- |
| **D**uplicate Line or Selection | Alt+D          | Ctrl+D          |                                                                   |
| **D**elete Line                 | Shift+Delete   | Shift+Delete    | Remove this shortcut for Cut action then assign it to Delete Line |
| **E**xtend Selection            | Ctrl+Shift+E   | Cmd+Shift+E     |                                                                   |
| **S**hrink Selection            | Ctrl+Shift+S   | Cmd+Shift+S     |                                                                   |
