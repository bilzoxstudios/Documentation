# JoinPlus

### 🧩 Parameters

| Key                     | Description                                                              |
|-------------------------|--------------------------------------------------------------------------|
| `<id>`                  | Unique identifier for the effect (used internally).                      |
| `display`               | The name shown in the GUI (supports color codes).                        |
| `permission`            | Permission node required to use this effect.                             |
| `structure.title`       | Title displayed to all players when joining.                             |
| `structure.subtitle`    | Subtitle displayed below the title.                                      |
| `structure.actionbar`   | Message shown in the action bar.                                         |
| `status.no-permission`  | Message shown when the player lacks the permission.                      |
| `status.click-select`   | Message shown when the player clicks to select this option.              |
| `status.already-select` | Message shown when the effect is already selected.                       |

### 🔎 Creation parameters in the .yml

```yaml
joinplus:
  <id>:
    display: "<Display Name>"
    permission: "<Permission Node>"
    structure:
      title: "<Title Message>"
      subtitle: "<Subtitle Message>"
      actionbar: "<Actionbar Message>"
    status:
      no-permission: "<No Permission Message>"
      click-select: "<Click to Select Message>"
      already-select: "<Already Selected Message>"
```
### 💻 Example defaults of the .yml

```yaml
sakura:
  display: "&d&lSakura"
  permission: bilzjoinplus.joinplus.sakura
  structure:
    title: "&#FF85D4🌺 &#FFADE2(player_name) &#FF85D4🌺"
    subtitle: "&fcherry blossom fell into the lobby"
    actionbar: "&d🌺 Say hello to &f &d🌺"
  status:
    no-permission: " &#FF3D3D⏩ You need rank &6&lBILZOX "
    click-select: " &#95FF7E⏩ Left-click to select plus "
    already-select: " &#FF3D3D⏩ Already selected plus "
```