![](https://clouless.github.io/macos-keyboard-remapping/v2/keyboard-layout-map.png?v2)


> I use a german PC Keyboard Layout mapped to Mac. Working under macOS Sierra.


&nbsp;

-----

### Installation

**Remap Left-Control and Right-Cmd with Karabiner Elements**

We remap these keys with [Karabiner Elements](https://github.com/tekezo/Karabiner-Elements) under macOS Sierra.

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/v2/karabiner-elements-remap.png?v3" width="80%"></p>

 * Remap left-ctrl to left-cmd
 * Remap right-cmd to right-alt
 * Remap `<` to `^`
 * Remap `^` to `<`

**Remap Keys in Keyboard Maestro**

We basically remap the following with [Keyboard Maestro](https://www.keyboardmaestro.com/main/).

:bangbang: Karabiner Elements remap already in place!

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/v2/keyboard-maestro-remap.png?v2" width="80%"></p>

It is then exported as Macro Library.
You can import the Macro Library:

  * :sparkles: **[clouless-german-keyboard-remap-macros.kmlibrary](https://raw.githubusercontent.com/clouless/macos-keyboard-remapping/master/clouless-german-keyboard-remap-macros.kmlibrary)**


*Notes: [macOS Special Chars German](https://www.die-tastenkombination.de/tastenkombinationen-mac-os-sonderzeichen.html)*

Special Application Specific Macros like `ctrl+c` in IntelliJ IDEA terminal are done like so:

https://github.com/clouless/macos-keyboard-remappingMacros

&nbsp;

**iTerm2**

Under 'Profiles' → 'Keys' add some key-combo 'send hex' remappings
to enable ctrl+d and ctrl+c.

| key combo | send hex | remapped to |
|------------|------------|--------|
| ⌘+c        | 0x03       | ctrl+c |
| ⌘+d        | 0x04       | ctrl+d |

-----

&nbsp;


**Limitations**

 * Once Safari creates a "Secure Input Mode", Keyboard Maestro is disabled.
   * Don't use safari


-----

&nbsp;

### License

[MIT](./LICENSE) © [Bernhard Grünewaldt](https://github.com/clouless)
