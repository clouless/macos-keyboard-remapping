# macos-keyboard-remapping

I use a german Windows Keyboard Layout mapped to Mac. Working under macOS Sierra.

![](https://clouless.github.io/macos-keyboard-remapping/keyboard-layout-map.png)



:bangbang: What is not working globally so far:

 * Jump Words with left-ctrl→ and left-ctrl←
   * works only with ⌥→ and ⌥←


&nbsp;

-----

## Remapping Left-Control and Right-Cmd with Karabiner Elements

We remap these two keys with [Karabiner Elements](https://github.com/tekezo/Karabiner-Elements) under macOS Sierra.

![](https://clouless.github.io/macos-keyboard-remapping/karabiner-elements-remap.png)

&nbsp;

-----

## Custom Keyboard Profile

I created a custom Keyboard Profile with [Ukulele](http://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&id=ukelele)

**NORMAL**


![](https://clouless.github.io/macos-keyboard-remapping/ukulele-normal.png)

**SHIFT**

![](https://clouless.github.io/macos-keyboard-remapping/ukulele-shift.png)

**ALT**

![](https://clouless.github.io/macos-keyboard-remapping/ukulele-alt.png)

&nbsp;

I had to modify the XML further for:

**Key `10`** which has `>`, `<` and `|` mapped

```
  <keyMapSet id="ANSI">
    <keyMap index="0">
      ...
      <key code="10" output="&#x003C;"/>
      ...
    </keyMap>
    <keyMap index="1">
      ...
      <key code="10" output="&#x003E;"/>
      ...
    </keyMap>
    <keyMap index="2">
      ...
      <key code="10" output="&#x007C;"/>
      # NOTE: Hex must have 4 Chars preceded by zeros if too short!
```



&nbsp;

-----

## Install Keyboard Layout in macOS Sierra


**(1)** Download **[clouless-german-keyboard-bundle-v11.bundle.zip](https://github.com/clouless/macos-keyboard-remapping/blob/master/clouless-german-keyboard-bundle-v11.bundle.zip?raw=true)** and extract


**(2)** Copy to `/Library/Keyboard Layouts/`

```
sudo su
cp -r clouless-german-keyboard-bundle.bundle /Library/Keyboard\ Layouts/
```

**(3)** Activate it in System Settings Keyboard:

![](https://clouless.github.io/macos-keyboard-remapping/activate-layout-01.png)

![](https://clouless.github.io/macos-keyboard-remapping/activate-layout-02.png?v3)


&nbsp;

----

## Office Mac e.g. Word

Word has some strange auto-language feature switching back to standard german.
But since I don't write code in Word, it is fine.


&nbsp;

----

## IntelliJ IDEA

'Preferences' → 'Keymap' Search for:

 * 'Move Caret to Next Word' and add Shortcut `left-ctrl→`
 * 'Move Caret to Previous Word' and add Shortcut `left-ctrl←`
 * 'Move Caret to Next Word with Selection' and add Shortcut `left-ctrl⇧→`
 * 'Move Caret to Previous Word with Selection' and add Shortcut `left-ctrl⇧←`

![](https://clouless.github.io/macos-keyboard-remapping/intellij-next-word.png)


## Atom.io

Work out of the box

-----

&nbsp;

## iTerm2


Under 'Profiles' → 'Keys' do:

| key combo | hex | remapped to |
|------------|------------|--------|
| ⌘+c        | 0x03       | ctrl+c |
| ⌘+d        | 0x04       | ctrl+d |



## Chrome

:bangbang: Home and End not working



## Creating the Keyboard Bundle

In Ukelele do 'New Layout Collection':

 * Add `clouless-german-keyboard-layout.keylayout`
 * Add Icon icns
 * Set languages and locale to german
 * Save as `clouless-german-keyboard-bundle-v11.bundle`

![](https://clouless.github.io/macos-keyboard-remapping/keyboard-bundle-01.png)

![](https://clouless.github.io/macos-keyboard-remapping/keyboard-bundle-02.png)

-----

&nbsp;

### License

[MIT](./LICENSE) © [Bernhard Grünewaldt](https://github.com/clouless)
