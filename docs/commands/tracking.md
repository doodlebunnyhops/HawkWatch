# 📡 Tracking Commands

These commands let you follow updates for specific Roblox games. You’ll receive alerts when the game changes — such as new thumbnails, descriptions, or update timestamps.

> ⚠️ You can only track up to 2 games at once. This may change in the future.

---

## 🔍 Start & Stop Tracking

### `/watch game`

**Description:**  
Start tracking updates for a game by name or ID. Only works in Text or Thread channels.

**Usage:**
```plaintext
/watch game name:<name|id> notify:<channel> ping_role:<role>
```

**Options:**
- `name` (*String or ID*, Required) — The game’s name or numeric ID.
- `notify` (*Channel*, Optional) — Where alerts will be sent. Defaults to current channel.
- `ping_role` (*Role to ping*, Optional) - Will ping this role on updates. **Last Update** Only posts will not ping!

**Examples:**
- `/watch game name:RIVALS`
- `/watch game name:17625359962`
- `/watch game name:RIVALS notify:updates`
- `/watch game name:RIVALS notify:updates ping_role:@rival_watchers`

---

### `/unwatch`

**Description:**  
Stop tracking a game.

> ❗ Unwatching a game prevents you from adding a new game for 1 hour. However, you can immediately rewatch the same game if it was a mistake.

**Usage:**
```plaintext
/unwatch name:<name|id>
```

**Options:**
- `name` (*String or ID*, Required) — The game’s name or numeric ID.

**Examples:**
- `/unwatch name:RIVALS`
- `/unwatch name:17625359962`

---

### `/unset role`

**Description:**  
Stop Receiving Pings on a tracked game

**Usage:**
```plaintext
/unset role game_name:<name>
```

**Options:**
- `name` (*String*) — The game’s name, it will populate which watched games that have ping roles assigned to them only.

**Examples:**
- `/unset role game_name:RIVALS`

---

## 📃 Manage & View Tracked Games

### `/list watched`

**Description:**  
List all games currently being tracked.

**Usage:**
```plaintext
/list watched post:<true|false>
```

**Options:**
- `post` (*Boolean*, Optional) — If `true`, posts the result so others can see. Defaults to `false`.

---

### `/watch settings set`

**Description:**  
Change what types of updates you want to receive for a specific game.

**Usage:**
```plaintext
/watch settings set game_name:<name|id> [options]
```

**Options:**
- `channel` (*Channel*, Optional) — Where to send alerts.
- `date` (*Track / Don't Track*, Optional) — Alert on update timestamps.
- `thumbnail` (*Track / Don't Track*, Optional) — Alert on thumbnail changes.
- `name` (*Track / Don't Track*, Optional) — Alert on name changes.
- `description` (*Track / Don't Track*, Optional) — Alert on description changes.

**Examples:**
- `/watch settings set game_name:Brookhaven 🏡RP channel:updates`
- `/watch settings set game_name:4924922222 thumbnail:Don't Track`
- `/watch settings set game_name:Brookhaven 🏡RP date:Don't Track name:Don't Track`

---

### `/watch settings get`

**Description:**  
View the current tracking settings for a game.

**Usage:**
```plaintext
/watch settings get game_name:<name|id>
```

**Options:**
- `name` (*String or ID*, Required) — The game’s name or numeric ID.

**Examples:**
- `/watch settings get game_name:Brookhaven 🏡RP`
- `/watch settings get game_name:17625359962`

---


[← Back to Commands](index.md)
