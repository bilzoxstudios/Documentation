# JoinMessages
Create personalized messages for privileged users

### Support
- Hex Color [Birdflop](https://www.birdflop.com/resources/rgb/)
- MiniMessage Format [Kyori](https://docs.advntr.dev/minimessage/format)
- PlaceholderAPI [BilzJoinPlus](https://docs.bilzox.es/bilzjoinplus-placeholders.html) & [Wiki](https://wiki.placeholderapi.com/users/placeholder-list/)

| Usage        | Description                                           |
|--------------|-------------------------------------------------------|
| `<id>`       | The id is to identify the cosmetic in the commands    |
| `display`    | Display the custom name of the cosmetic               |
| `permission` | Add a permission to the cosmetic to make it exclusive |
| `message`    | Place an exclusive and modern message                 |
| `status`     | Modify the messages of the placeholder variables      |

### Structure
```yaml
joinmessages:
  <id>:
    display: "Display custom text name"
    permission: Insert permission
    message:
      - "Insert custom text"
    status:
      no-permission: "This is part of the placeholder (%\bjpstatus%)"
      click-select: "This is part of the placeholder (%\bjpstatus%)"
      already-select: "This is part of the placeholder (%\bjpstatus%)"
```

### Example cosmetics.yml
```yaml
joinmessages:
  halloween:
    display: "&eHalloween"
    permission: bilzjoinplus.joinmessage.halloween
    message:
      - "&#FF7518🎃 Trick or Treat! &e%\player_name% &#FF7518rises from the shadows! &#FF7518👻"
    status:
      no-permission: " &#FF3D3D⏩ You need rank &6&lBILZOX "
      click-select: " &#95FF7E⏩ Left-click to select message "
      already-select: " &#FF3D3D⏩ Already selected message "
```

### Preview
![Preview](JoinMessagePreview.png)
