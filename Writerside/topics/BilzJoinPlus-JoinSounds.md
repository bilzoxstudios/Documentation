# JoinSounds

### 🧩 Parameters

| Key                    | Description                                                            |
|------------------------|------------------------------------------------------------------------|
| `<id>`                 | Unique identifier for the sound (used internally).                     |
| `display`              | The name shown in the GUI (supports color codes).                      |
| `sound`                | A valid XSound enum name.                                              |
| `permission`           | Custom permission required to unlock this sound.                       |
| `status.no-permission` | Message shown when player lacks the permission.                        |
| `status.click-select`  | Message shown when the player clicks to select this option.            |
| `status.already-select`| Message shown when the sound is already selected.                      |

### 🔎 Creation parameters in the .yml

```yaml
joinsounds:
  <id>:
    display: "<Display Name>"
    sound: "<XSound Enum>"
    permission: "<Permission Node>"
    status:
      no-permission: "<No Permission Message>"
      click-select: "<Click to Select Message>"
      already-select: "<Already Selected Message>"
```

### 💻 Example defaults of the .yml

```yaml
dragon:
  display: "&aDragon"
  sound: "ENTITY_ENDERDRAGON_GROWL"
  permission: bilzjoinplus.joinsound.dragon
  status:
    no-permission: " &#FF3D3D⏩ You need rank &6&lBILZOX "
    click-select: " &#95FF7E⏩ Left-click to select sound "
    already-select: " &#FF3D3D⏩ Already selected sound "
```