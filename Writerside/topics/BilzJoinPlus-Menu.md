# Menu

This file defines the configuration for the cosmetics menu GUI, used to display and interact with join effects, sounds, messages, and more in **BilzJoin+**.

The menu is fully customizable using:
- ✅ `XMaterial` for item types
- ✅ `XSound` for sound effects
- ✅ `PlaceholderAPI` support for dynamic content
- ✅ Legacy color codes (`&`), hex colors (`&#RRGGBB`), and MiniMessage formatting

### 🧩 Parameters

| Key           | Description                                                                 |
|---------------|-----------------------------------------------------------------------------|
| `menu.title`  | Title of the GUI menu (supports HEX, legacy `&` codes, and PlaceholderAPI).|
| `menu.size`   | Number of rows in the inventory (1–6, each row has 9 slots).                |
| `items.<id>`  | Unique identifier for each item in the menu.                               |
| `name`        | Display name of the menu item (supports HEX, & codes, MiniMessage, PAPI).  |
| `slot`        | Slot index where the item is placed (0 to 53).                             |
| `slots`          | Multiple slot indexes where the item is duplicated (use list of integers). |
| `material`    | XMaterial enum name (e.g., `JUKEBOX`, `DIAMOND`).                          |
| `lore`        | Tooltip text shown on hover (multi-line, full formatting supported).       |
| `left-click`  | List of actions executed on left-click.                                    |
| `right-click` | List of actions executed on right-click.                                   |

---

## 📄 Menu Structure

```yaml
menu:
  title: "<String> # Title displayed at the top of the GUI (supports HEX, legacy &, PlaceholderAPI)"
  size: <Integer> # Number of rows in the menu (1–6). Each row contains 9 slots (9–54 total)

items:
  <id>:
    name: "<String> # Display name of the item (supports HEX, legacy &, MiniMessage, PAPI)"
    slot: <Integer> # (Optional) Single slot index (0–53) where this item will appear
    slots:          # (Optional) List of slot indexes (for multiple-slot display)
      - <Integer>   # Example: 10
      - <Integer>   # Example: 11
    material: "<XMaterial> # Item type using a valid XMaterial enum name"
    lore:
      - "<String> # Tooltip line 1 (supports placeholders, HEX, & codes)"
      - "<String> # Tooltip line 2"
    left-click:
      - "[ACTION] <value> # Actions executed on left-click"
    right-click:
      - "[ACTION] <value> # Actions executed on right-click"
```

## 💽 Actions

| Key         | Description                                                       |
|-------------|-------------------------------------------------------------------|
| `[CLOSE]`   | Close the menu                                                    |
| `[COMMAND]` | Execute commands as the user (PAPI support)                       |
| `[SOUND]`   | Play sounds, you can also modify volume and pitch                 |
| `[MESSAGE]` | User Messages (Accepts all color formats and PAPI)                |

---