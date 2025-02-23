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
* For adding new shortcuts, avoid using the main modifier key of Mnemonic Keymap (Ctrl on Windows and Command on MacOS).
  Usually, I use Alt on Windows and Ctrl on MacOS for my new personal shortcuts.

| Action                      | Windows | MacOS  |
| --------------------------- | ------- | ------ |
| Duplicate Line or Selection | Alt+D   | Ctrl+D |
| Delete Line                 | Alt+X   | Ctrl+X |
