# arcdps_buffbar

<img width="512" height="384" alt="arcdps_buffbar" src="https://github.com/user-attachments/assets/a4a4e7ff-7850-43ef-8736-4bb738df3202" />

<br/><br/>
`arcdps_buffbar` is an ArcDPS addon for Guild Wars 2 that provides a customizable self-buff overlay.

The overlay can show:

- most effects: boons, auras, relics, skill effects, etc
- stack counts
- visible remaining-duration timers
- duration bars
- source indicators (dots) for self vs ally-applied effects
- horizontal or vertical layouts


### Installation

1. Install [ArcDPS](https://www.deltaconnected.com/arcdps/) for Guild Wars 2.
2. Download `arcdps_buffbar.dll` from the releases section.
3. Place the DLL in your GW2 addon folder:

```text
Guild Wars 2\addons\arcdps_buffbar.dll
```

Restart Guild Wars 2 after installing or updating the addon.


### Files

The addon stores settings and cache files under:

```text
Guild Wars 2\addons\arcdps_buffbar\
```

The main settings file is:

```text
Guild Wars 2\addons\arcdps_buffbar\arcdps_buffbar.ini
```

The icon and effect cache is stored in:

```text
Guild Wars 2\addons\arcdps_buffbar\cache\
```


### Configuration

Open the ArcDPS options panel and find the `arcdps_buffbar` tab.

The important setting is the overlay mode:

- `Off`: hides the buff bar.
- `On`: shows your pinned effects.
- `Configure`: opens a picker of currently active effects so you can add or remove pins. Requires having the active effect.

Pins are the effects the buff bar tracks. In normal mode, the overlay only shows pinned effects. If a pinned effect is inactive, it stays in its slot as a dimmed icon.

To populate pins:

1. Set the overlay to `Configure`.
2. Apply or receive the boon, aura, or effect you want to track.
3. Click the effect in the configure picker to pin it.
4. Switch the overlay back to `On`.

You can also add pins manually by entering an effect ID in the Pins section. The Known Effects window can help find common effect IDs.

Pin scope controls where pins apply:

- `Global`: same pins everywhere.
- `Current profession`: separate pins per profession.
- `Current elite specialization`: separate pins per elite specialization.

Other options control icon size, spacing, opacity, orientation, timer text, duration bars, stack text, source indicators, and whether unknown effects are shown.

When the overlay is unlocked, you can move it by dragging the buff bar. Right-click the unlocked overlay for quick lock and save actions.
