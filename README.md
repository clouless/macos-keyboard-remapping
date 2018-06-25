![](https://clouless.github.io/macos-keyboard-remapping/v2/keyboard-layout-map.png?v2)


> I use a german PC Keyboard Layout mapped to Mac. Working under macOS Sierra.



&nbsp;

-----

### Features


|key-combo | result |
|----------|--------|
| left-ctrl+c | copy text to clipboard |
| left-ctrl+x | cut text to clipboard |
| left-ctrl+v | paste text from clipboard |
| left-ctrl+shift+right | marks text one word to right |
| left-ctrl+shift+left | marks text one word to left |
| left-ctrl+a | select all |
| left-ctrl+s | save |
| left-⌘+e    | opens Path Finder Application |
| left-ctrl+shift+eject    | go to sleep mode |
| right-⌘+q   | @ |
| right-⌘+e   | € |
| right-⌘+7   | { |
| right-⌘+8   | [ |
| right-⌘+9   | ] |
| right-⌘+0   | } |
| right-⌘+ß   | \ |
| right-⌘++   | ~ |
| right-⌘+<   | &#x01C0; |


&nbsp;

-----

### Usage

We do not need *Karabiner* or *Karabiner Elements* anymore! **Keyboard Maestro does all the work** :fire:

#### :musical_keyboard: Remap key combinations with Keyboard Maestro

We basically remap the following with [Keyboard Maestro](https://www.keyboardmaestro.com/main/).

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/v2/keyboard-maestro-remap.png?v2" width="80%"></p>

You can import the Macro Library:

  * :sparkles: **[clouless-german-keyboard-remap-macros.kmlibrary](https://raw.githubusercontent.com/clouless/macos-keyboard-remapping/master/clouless-german-keyboard-remap-macros.kmlibrary)**


*Notes: [macOS Special Chars German](https://www.die-tastenkombination.de/tastenkombinationen-mac-os-sonderzeichen.html)*


&nbsp;

-----

### Limitations

 * Once Safari creates a "Secure Input Mode", Keyboard Maestro is disabled.
 * To paste passwords into password input fileds you cannot use CTRL+V and need to use CMD+V
 * Mission Control default Shortcuts need to be disabled to avoid conflicts:

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/v2/deactivate-mission-control-shortcuts.png" width="80%"></p>

-----

&nbsp;

### License

[MIT](./LICENSE) © [Bernhard Grünewaldt](https://github.com/clouless)
