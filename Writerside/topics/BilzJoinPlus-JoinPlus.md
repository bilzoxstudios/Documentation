# JoinPlus
Create titles and actionbars for users with permissions

### Support
- Hex Color [Birdflop](https://www.birdflop.com/resources/rgb/)
- MiniMessage Format [Kyori](https://docs.advntr.dev/minimessage/format)
- PlaceholderAPI [BilzJoinPlus](https://docs.bilzox.es/bilzjoinplus-placeholders.html) & [Wiki](https://wiki.placeholderapi.com/users/placeholder-list/)

| Usage                 | Description                                            |
|-----------------------|--------------------------------------------------------|
| `<id>`                | The id is to identify the cosmetic in the commands     |
| `display`             | Display the custom name of the cosmetic                |
| `permission`          | Add a permission to the cosmetic to make it exclusive  |
| `structure.title`     | Customize the text that is displayed on the screen     |
| `structure.subtitle`  | Customize the subtitle that is displayed on the screen |
| `structure.actionbar` | Modify the message that appears above the hotbar       |
| `status`              | Modify the messages of the placeholder variables       |

### Structure
```yaml
joinplus:
  <id>:
    display: "Display custom text name"
    permission: Insert permission
    structure:
      title: "Insert a title"
      subtitle: "Insert subtitle"
      actionbar: "Insert actionbar"
    status:
      no-permission: "This is part of the placeholder (%\bjpstatus%)"
      click-select: "This is part of the placeholder (%\bjpstatus%)"
      already-select: "This is part of the placeholder (%\bjpstatus%)"
```

### Example cosmetics.yml
```yaml
joinplus:
  zeus:
    display: "&cZeus"
    permission: bilzjoinplus.joinplus.zeus
    structure:
      title: "&e&l⚡ &6%\player_name% &e&l⚡"
      subtitle: "&fThe heir of Zeus entered"
      actionbar: "&eGreet the heir of Zeus: &6%\player_name%"
    status:
      no-permission: " &#FF3D3D⏩ You need rank &6&lBILZOX "
      click-select: " &#95FF7E⏩ Left-click to select plus "
      already-select: " &#FF3D3D⏩ Already selected plus "
```

### Preview
![Preview](JoinPlusPreview.png)