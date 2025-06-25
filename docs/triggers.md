
## 🔔 What Can Trigger a HawkWatch Alert?

HawkWatch watches for several types of changes to a Roblox experience. You can choose which ones matter to you — and the bot will only alert you for the parts you’ve selected.

By default, HawkWatch tracks:

- ✅ **Update time**
- ✅ **Name changes**
- ✅ **Thumbnail changes**
- ✅ **Description changes**

You can customize your preferences at any time.

---

### 🕒 1. **Update Time**

This is the most common trigger for an alert.

Roblox updates an experience’s "last updated" time when the developer:
- Publishes a new version of the main game (usually the first place players join)
- Updates other **public places** within the experience (joinable or visible to players)
  - This can include places that are not directly playable, but are **listed publicly on roblox.com**.
- Makes structural or ownership-level changes (like transferring the experience to a group)

It's important to know:  
🔹 **Not every update means new gameplay**. Developers often:
- Push **code changes that are hidden from players** (like feature flags or internal systems)
- Release **bug fixes or performance tweaks** that don’t visibly change the game
- Update metrics, analytics, or server behavior without changing the experience’s look or feel

In short: **if the change affects what players can access or see — or how the game runs under the hood — it can result in a new update time**, and HawkWatch will catch it.


---

### ✏️ 2. **Name Changes**

If the developer changes the experience’s title — even slightly — HawkWatch will detect it.

This is useful for spotting:
- New updates being teased
- Event names or seasonal changes
- Sudden rebrands


---

### 🖼️ 3. **Thumbnail Changes**

HawkWatch tracks visual thumbnail changes using Roblox’s thumbnail API. These images are usually what you see on the game’s main page.

Thumbnails are often changed during:
- Seasonal events or promotions
- Major updates
- Style refreshes

Note: **Thumbnail changes do not always mean the game was updated** — developers can update them separately.

---

### 📄 4. **Description Changes**

Changes to the game’s description can signal:
- Patch notes or update logs
- New features being introduced
- Promotional text changes

If a developer edits the description, HawkWatch will compare it and notify you.

---

### ⚙️ Customize What You Track

If you only care about thumbnails and names? No problem.
Want just timestamp-based alerts? Totally fine.

You’re in control of what HawkWatch watches for every game you follow.

[← Back to Documentation](index.md)
