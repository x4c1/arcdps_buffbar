# arcdps_buffbar

<img width="400" alt="arcdps_buffbar" src="https://github.com/user-attachments/assets/a4a4e7ff-7850-43ef-8736-4bb738df3202" />
<img width="440" alt="skillbars" src="https://github.com/user-attachments/assets/9b61845c-c814-48bb-84b6-7d1ff4c3b856" />
<br/><br/>

`arcdps_buffbar` is an ArcDPS addon for Guild Wars 2 that provides customizable self-buff overlays.

The overlay can show:

- multiple independent buff bars
- most effects: boons, auras, relics, conditions, etc
- weapon/profession/utility slot cooldowns
- stack counts
- visible remaining-duration timers
- duration bars
- source indicators (dots) for self vs ally-applied effects


### Installation

1. Install [ArcDPS](https://www.deltaconnected.com/arcdps/) for Guild Wars 2.
2. Download `arcdps_buffbar.dll` from the releases section.
3. Place the DLL in your GW2 addon folder:

```text
Guild Wars 2\addons\arcdps_buffbar.dll
```

Restart Guild Wars 2 after installing or updating the addon.


### Configuration

Open the ArcDPS options panel and find the `arcdps_buffbar` tab.

The important setting is the overlay mode:

- `Off`: hides all buff bars.
- `On`: shows your enabled buff bars.
- `Configure`: opens `Configure Mode - Active Effects` window, a floating picker of currently active effects.

Pins are the effects a buff bar tracks. In normal mode, each enabled bar only shows its own pinned effects. If a pinned effect is inactive, it stays in its slot as a dimmed icon.

Each bar has its own pins and layout settings, including name, enabled state, icon size, spacing, opacity, lock state, horizontal or vertical orientation, title bar visibility, and screen position.

In configure mode, every enabled buff bar temporarily shows its title bar. Changes in the configuration panel apply to the selected bar.

To populate pins:

1. Set the overlay to `Configure`.
2. Apply or receive the boon, aura, or effect you want to track.
3. Select the buff bar you want to edit by grabbing its title bar.
4. Click or drag an effect in `Configure Mode` window to pin or unpin it on the selected bar.
6. Switch the overlay back to `On`.

Manage pins directly on the bars while in configure mode:

- right-click a bar title to lock/unlock that bar
- right-click a pinned icon for remove actions
- drag pinned icons left, right, up, or down to reorder them
- drag pinned icons between buff bars to move them

Add pins manually by entering an effect ID in the Pins section. The Known Effects window can help find common effect IDs.

Pin scope controls where pins apply:

- `Global`: same pins everywhere.
- `Current profession`: separate pins per profession.
- `Current elite specialization`: separate pins per elite specialization.

Other options control icon size, spacing, opacity, orientation, timer text, duration bars, stack text, source indicators, and whether unknown effects are shown.


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


