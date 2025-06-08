# Placeholders

**Category**
- JoinSounds - `Cosmetic:` All those you created
- JoinPlus - `Cosmetic:` All those you created
- JoinMessages - `Cosmetic:` All those you created
- JoinEffects - `Cosmetic:` The 10 default effects

`FIREWORKS, THUNDER, WOOLS, TNT, FLOWER, BURST, BATS, SQUID, NOTES, WITHER`

| Placeholder                                   | Description                                                |
|-----------------------------------------------|------------------------------------------------------------|
| `%bjpprogress_(category)_progress_percent%`   | Displays a % of completed cosmetics                        |
| `%bjpprogress_(category)_progress_total%`     | Displays the full cosmetic number                          |
| `%bjpprogress_(category)_progress_unlocked%`  | Displays the number of unlocked cosmetics                  |
| `%bjpprogress_(category)_progress_bar%`       | Displays a completion bar                                  |
| `%bjpstatus_(category)_status_(cosmetic)%`    | Button to show if it is locked, selected or you can select |
| `%bjpcosmetic_status_(category)_(cosmetic)%`  | Shows if you have Locked/Unlocked the cosmetic             |

### Configurable
```YAML
config:
  status:
    locked: "&#FF0000[Locked... 🔒]"
    unlocked: "&#00FF11[Unlocked... 🔓]"
  total:
    format: "&a%\unlocked%/%\total%"
    no-data: "&cX/X"
  progress:
    bar:
      length: 7
      char: "○"
      color-filled: "&a"
      color-unfilled: "&7"
      brackets:
        left: "&7["
        right: "&7]"
      no-data: "&7[&c?&7]"
    percent:
      decimal: false
      color: "&#99A4FF"
      brackets:
        left: "("
        right: ")"
      no-data: "&c0%"
```

### Upcoming Placeholders
| Placeholder                     | Description                                                 |
|---------------------------------|-------------------------------------------------------------|
| `%bjpselected_(category)%`      | Shows which cosmetic you have selected                      |
| `%bjplist_selected_(category)%` | Displays a complete list of the cosmetics you have selected |