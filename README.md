![](https://clouless.github.io/macos-keyboard-remapping/v2/keyboard-layout-map.png?v2)


> I use a german PC Keyboard Layout mapped to Mac. Working under macOS Sierra.


&nbsp;

-----

### Usage

#### :musical_keyboard: Remap single keys with Karabiner Elements

We remap these keys with [Karabiner Elements](https://github.com/tekezo/Karabiner-Elements) under macOS Sierra.

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/v2/karabiner-elements-remap.png?v3" width="80%"></p>

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

### Application Customization

**iTerm2**

Under 'Profiles' → 'Keys' add some key-combo 'send hex' remappings
to enable ctrl+d and ctrl+c.

| key combo | send hex | remapped to |
|------------|------------|--------|
| ⌘+c        | 0x03       | ctrl+c |
| ⌘+d        | 0x04       | ctrl+d |

&nbsp;


### Limitations

 * Once Safari creates a "Secure Input Mode", Keyboard Maestro is disabled.
   * Don't use safari
 * IntelliJ embedded terminal CTRL+C not working  


-----

&nbsp;

### License

[MIT](./LICENSE) © [Bernhard Grünewaldt](https://github.com/clouless)
