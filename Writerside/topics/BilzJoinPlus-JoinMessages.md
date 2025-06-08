# JoinMessages

### 🧩 Parameters

| Key                    | Description                                                            |
|------------------------|------------------------------------------------------------------------|
| `<id>`                 | Unique identifier for the message (used internally).                   |
| `display`              | The name shown in the GUI (supports color codes).                      |
| `permission`           | Permission node required to use this join message.                     |
| `message`              | A list of formatted message lines (supports color codes and placeholders). |
| `status.no-permission` | Message shown when player lacks the permission.                        |
| `status.click-select`  | Message shown when the player clicks to select this option.            |
| `status.already-select`| Message shown when the message is already selected.                    |

### 🔎 Creation parameters in the .yml

```yaml
joinmessages:
  <id>:
    display: "<Display Name>"
    permission: "<Permission Node>"
    message:
      - "<Line 1 of the message>"
      - "<Line 2 (optional)>"
    status:
      no-permission: "<No Permission Message>"
      click-select: "<Click to Select Message>"
      already-select: "<Already Selected Message>"
```

### 💻 Example defaults of the .yml

```yaml
joinmessages:
  halloween:
    display: "&eHalloween"
    permission: bilzjoinplus.joinmessage.halloween
    message:
      - "&#FF7518🎃 Trick or Treat! &e(player_name) &#FF7518rises from the shadows! &#FF7518👻"
    status:
      no-permission: " &#FF3D3D⏩ You need rank &6&lBILZOX "
      click-select: " &#95FF7E⏩ Left-click to select message "
      already-select: " &#FF3D3D⏩ Already selected message "
```