# Configurations

### Database
> Types: YAML - SQLite - MySQL
```YAML
database:
  type: "<insert type>"
  config:
    user: "root"
    password: "password"
    host: "localhost"
    database: "bilzjoinplus"
    port: 3306
```

### JoinItem
Customize the default item to open cosmetics

| Types of Materials      |                                                                                                                      |
|-------------------------|----------------------------------------------------------------------------------------------------------------------|
| XMaterial               | [Wiki](https://github.com/CryptoMorin/XSeries/blob/master/core/src/main/java/com/cryptomorin/xseries/XMaterial.java) |
| `basehead-<64>`         | Custom heads base64                                                                                                  |
| `skull-%\player_name% ` | The player's head appears                                                                                            |
| `url-<url> `            | Custom heads from textures.minecraft.net                                                                             |

```YAML
join-item:
  switch: true
  hotbar-slot: <0 - 8>
  material: <Material>
  name: "&#FF651B&lBilzJoin+ &7| &#FFAF89(Right Click)"
  lore:
    - '&7Thank you for purchasing the BilzJoin+ Premium!'
  left-click:
    - '[COMMAND] bilzjoin menu open joineffects.yml'
  right-click:
    - '[COMMAND] bilzjoin menu open joineffects.yml'
```