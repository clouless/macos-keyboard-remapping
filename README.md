![](https://clouless.github.io/macos-keyboard-remapping/keyboard-layout-map.png)


> I use a german Windows Keyboard Layout mapped to Mac. Working under macOS Sierra.



&nbsp;

-----

### Installation

**Install Keyboard Layout in macOS Sierra**


**(1)** Download **[clouless-german-keyboard-bundle-v11.bundle.zip](https://github.com/clouless/macos-keyboard-remapping/blob/master/clouless-german-keyboard-bundle-v11.bundle.zip?raw=true)** and extract


**(2)** Copy to `/Library/Keyboard Layouts/`

```
sudo su
cp -r clouless-german-keyboard-bundle.bundle /Library/Keyboard\ Layouts/
```

**(3)** Activate it in System Settings Keyboard:

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/activate-layout-01.png" width="80%"></p>

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/activate-layout-02.png?v3" width="80%"></p>


&nbsp;

**Remap Left-Control and Right-Cmd with Karabiner Elements**

We remap these two keys with [Karabiner Elements](https://github.com/tekezo/Karabiner-Elements) under macOS Sierra.

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/karabiner-elements-remap.png" width="80%"></p>

&nbsp;

-----


### Adjust Applications


**Microsoft Office Mac**

Word has some strange auto-language feature switching back to standard german.
But since I don't write code in Word, it is fine.


&nbsp;

**IntelliJ IDEA**

'Preferences' → 'Keymap' Search for:

 * 'Move Caret to Next Word' and add Shortcut `left-ctrl→`
 * 'Move Caret to Previous Word' and add Shortcut `left-ctrl←`
 * 'Move Caret to Next Word with Selection' and add Shortcut `left-ctrl⇧→`
 * 'Move Caret to Previous Word with Selection' and add Shortcut `left-ctrl⇧←`

<p align="center"><img src="https://clouless.github.io/macos-keyboard-remapping/intellij-next-word.png" width="80%"></p>

&nbsp;

**Atom.io**

:bangbang: Jump words not working!

&nbsp;

**iTerm2**

Under 'Profiles' → 'Keys' add some key-combo 'send hex' remappings:

| key combo | send hex | remapped to |
|------------|------------|--------|
| ⌘+c        | 0x03       | ctrl+c |
| ⌘+d        | 0x04       | ctrl+d |


&nbsp;

**Chrome**

:bangbang: Home and End not working
:bangbang: Jump words not working!

&nbsp;

**GLOBALLY**

:bangbang: What is not working globally so far:

 * Jump Words with left-ctrl→ and left-ctrl←
   * works only with ⌥→ and ⌥←

-----

&nbsp;

### Technical Documentation

See [Howto create the custom Keyboard Layout Bundle](./TECHDOC.md)

-----

&nbsp;

### License

[MIT](./LICENSE) © [Bernhard Grünewaldt](https://github.com/clouless)
