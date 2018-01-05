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

#### :musical_keyboard: Remap single keys with Karabiner Elements

We remap these keys with [Karabiner Elements](https://github.com/tekezo/Karabiner-Elements) under macOS Sierra.

Since `All Devices` does not seem to apply for internal Keyboard, we need to set
things explicitly for the internal Keyboard.

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/v2/karabiner-all-devices.png?v3" width="80%"></p>

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/v2/karabiner-internal-keyboard.png?v3" width="80%"></p>

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/v2/karabiner-extern-usb.png?v4" width="80%"></p>

 * Remap left-ctrl to left-cmd
 * Remap right-cmd to right-alt
 * Remap `<` to `^`
 * Remap `^` to `<`

&nbsp;

#### :musical_keyboard: Remap key combinations with Keyboard Maestro

We basically remap the following with [Keyboard Maestro](https://www.keyboardmaestro.com/main/).

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/v2/keyboard-maestro-remap.png?v2" width="80%"></p>

You can import the Macro Library:

  * :sparkles: **[clouless-german-keyboard-remap-macros.kmlibrary](https://raw.githubusercontent.com/clouless/macos-keyboard-remapping/master/clouless-german-keyboard-remap-macros.kmlibrary)**


*Notes: [macOS Special Chars German](https://www.die-tastenkombination.de/tastenkombinationen-mac-os-sonderzeichen.html)*


&nbsp;

-----

### Application Customization

**iTerm2**

Under 'Profiles' → 'Keys' add some key-combo 'send hex' remappings
to enable ctrl+d and ctrl+c.

| key combo | send hex | remapped to |
|------------|------------|--------|
| ⌘+c        | 0x03       | ctrl+c |
| ⌘+d        | 0x04       | ctrl+d |


&nbsp;

**IntelliJ IDEA**

Add a shortcut ⌘+SPACE for code completition.


<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/v2/intellij-complete-basic.png?v3" width="80%"></p>

&nbsp;

**Spotlight**

Deactivate alle Spotlight shortcuts, since we use Alfred anyway.

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/v2/spotlight-deactivate.png?v3" width="80%"></p>


&nbsp;

-----

### Limitations

 * Once Safari creates a "Secure Input Mode", Keyboard Maestro is disabled.
   * Don't use safari
 * IntelliJ embedded terminal CTRL+C not working  


-----

&nbsp;

### License

[MIT](./LICENSE) © [Bernhard Grünewaldt](https://github.com/clouless)
