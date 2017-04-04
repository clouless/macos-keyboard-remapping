# macos-keyboard-remapping

I use a german Windows Keyboard Layout mapped to Mac.

Until macOS Sierra I did this via Karabiner, but since Karabiner is broken in macOS Sierra, I have some workarounds now.

&nbsp;

-----


## Keyboard Layout

![](https://clouless.github.io/macos-keyboard-remapping/keyboard-layout-map.png)


&nbsp;

-----

## Remapping Left-Control and Right-Cmd with Karabiner Elements

We remap these two keys with [Karabiner Elements](https://github.com/tekezo/Karabiner-Elements) under macOS Sierra.

![](https://clouless.github.io/macos-keyboard-remapping/karabiner-elements-remap.png)

&nsbp;

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
			<key code="10" output="<"/>
   ...
		</keyMap>
		<keyMap index="1">
  ...
			<key code="10" output=">"/>
  ...
```
