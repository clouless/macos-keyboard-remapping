# Howto create the custom Keyboard Layout Bundle

## 1. Custom Keyboard Layout

I created a custom Keyboard Layout with [Ukulele](http://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&id=ukelele)

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

## 2. Custom Keyboard Bundle (includes locale and icon)

In Ukelele do 'New Layout Collection':

 * Add `clouless-german-keyboard-layout.keylayout`
 * Add Icon icns
 * Set languages and locale to german
 * Save as `clouless-german-keyboard-bundle-v11.bundle`

![](https://clouless.github.io/macos-keyboard-remapping/keyboard-bundle-01.png)

![](https://clouless.github.io/macos-keyboard-remapping/keyboard-bundle-02.png)
