# BilzMenu
![bilzmenu-api](https://img.shields.io/badge/bilzmenu-0.2.2-blue) ![Status](https://img.shields.io/badge/status-beta-yellow)

<warning>
Use this section to create multiple pages of your cosmetics, not for other things
</warning>

### How do I create another menu?
Go to the `BilzJoinPlus/menus/` folder and create a `<name>.yml`

You have 2 options to load the new menu
- `/bilzjoinplus reload menus`
- `/bilzjoinplus menu reload <name>.yml`

### Menu structure
- Hex Color [Wiki](https://www.birdflop.com/resources/rgb/)
- XMaterial [Wiki](https://github.com/CryptoMorin/XSeries/blob/master/core/src/main/java/com/cryptomorin/xseries/XMaterial.java)
- XSound [Wiki](https://github.com/CryptoMorin/XSeries/blob/master/core/src/main/java/com/cryptomorin/xseries/XSound.java)
- MiniMessage Format [Wiki](https://docs.advntr.dev/minimessage/format)
- PlaceholderAPI [BilzJoinAPI](https://docs.bilzox.es/bilzjoinplus-placeholders.html) & [Wiki](https://wiki.placeholderapi.com/users/placeholder-list/)
```YAML
menu:
  title: 'Name of your menu'
  size: 1 * 6

items:
  <id>:
    name: 'Enter a display'
    # Static Slot
    slot: <Insert a slot>
    # Multiple Slots
    slots:
      - <slot>
      - <slot>
    material: '<Material>'
    lore:
      - 'Insert a lore'
    left-click:
      - '[<ACTION>]'
    right-click:
      - '[<ACTION>]'
```

### Slots
<img src="SlotsInventory.png" alt="" width="400" height="400" />

### Actions
| Action Tag       | Description                                                                                                                                                                              |
|------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `[CLOSE]`        | Closes the player's current inventory.                                                                                                                                                   |
| `[SOUND]`        | Plays a sound at the player's location. Format: `[SOUND] <SOUND_NAME>:<VOLUME>:<PITCH>` (volume and pitch are optional, default 1.0). If it fails, sends an error message to the player. |
| `[MESSAGE]`      | Sends a chat message to the player. Supports placeholders and color codes. Format: `[MESSAGE] <text>`                                                                                    |
| `[COMMAND]`      | Executes a command as the player. Supports placeholders. Format: `[COMMAND] <command>`                                                                                                   |