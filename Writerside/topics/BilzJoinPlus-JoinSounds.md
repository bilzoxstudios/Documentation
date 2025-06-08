# JoinSounds
Create unique and exclusive sounds for privileged users

### Support
- Hex Color [Birdflop](https://www.birdflop.com/resources/rgb/)
- XSound [XSeries Github](https://github.com/CryptoMorin/XSeries/blob/master/core/src/main/java/com/cryptomorin/xseries/XSound.java)
- MiniMessage Format [Kyori](https://docs.advntr.dev/minimessage/format)

| Usage        | Description                                                  |
|--------------|--------------------------------------------------------------|
| `<id>`       | The id is to identify the cosmetic in the commands           |
| `display`    | Display the custom name of the cosmetic                      |
| `permission` | Add a permission to the cosmetic to make it exclusive        |
| `sound`      | Insert the sound you want and sound exclusive or mysterious  |
| `status`     | Modify the messages of the placeholder variables             |

### Structure
```yaml
joinsounds:
  <id>:
    display: "Display custom text name"
    permission: Insert permission
    sound: "Insert new sound"
    status:
      no-permission: "This is part of the placeholder (%\bjpstatus%)"
      click-select: "This is part of the placeholder (%\bjpstatus%)"
      already-select: "This is part of the placeholder (%\bjpstatus%)"
```

### Example cosmetics.yml
```yaml
joinsounds:
  cat:
    display: "&aCat"
    sound: "CAT_MEOW"
    permission: bilzjoinplus.joinsound.cat
    status:
      no-permission: " &#FF3D3D⏩ You need rank &6&lBILZOX "
      click-select: " &#95FF7E⏩ Left-click to select sound "
      already-select: " &#FF3D3D⏩ Already selected sound "
```