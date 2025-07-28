# 📝 HawkWatch Changelog

This changelog covers major updates and bug fixes that impact how users experience HawkWatch.

---

## [v1.2.6] – Smarter Pings and Faster Tracking  
- ⏱️ Tracking interval reduced to 1 minute for snappier update detection  
- 📢 Added per-game ping role support with `/watch settings set ping_role:@role`  
- 🔕 Ping roles are now ignored when the only change is a timestamp update  
- 🗓️ Added in-post “Disable Date Tracking” buttons for easier noise control  
- 🎮 Added occasional “Play Game” buttons to jump into updated games instantly  

---

## [v1.2.5] – API Reliability

- 🔐 Fixed Roblox API compatibility issues after SSL trust level changes from Roblox system.

---

## [v1.2.4] – Tracking Stability and Messaging Improvements

- 🧭 Improved timestamp logic to reduce false "update" alerts caused by minor time mismatches
- 🛠️ Made universe ID lookups more reliable during game tracking
- 🔗 Updated support server links in help and error messages

---

## [v1.2.3] – Permission Check Fixes

- ✅ Bot now validates whether it can post in target channels before confirming a watch or settings change
- 🧪 Reduced setup confusion when permissions are misconfigured

---

## [v1.2.2] – Channel Routing, Reliability, and Quality-of-Life Fixes

- ➕ You can now route update alerts to a different channel than where `/watch` was run
- 💬 `/list watched` can now post results publicly or reply privately
- 🛠️ Fixed false alerts caused by minor timestamp shifts (Roblox API-level seconds mismatches)
- 🛠️ Fixed settings reset bug when changing alert channels — settings now persist as expected
- ❌ News/Announcement channels are no longer supported for tracking
- 🔄 `/help` now reflects updated command behavior

---

## [v1.2.1] – Role Compatibility Improvement

- 🛡️ Added better detection for users with `administrator` permissions — resolves issues where some admins couldn't use commands
- ⏱️ Minor improvements to internal update timing for faster checks

---

## [v1.2.0] – 🟢 Public Launch (Multi-Server Support)

> First version where HawkWatch became available for use in any server.

- 🌐 Multi-server support added
- 🔎 Search filters out games already tracked
- ⚙️ Server-specific game settings and alert configurations supported
- 👁️ Improved visual alert handling (name, thumbnail, description, update time)

---

## Earlier Versions (v1.1.x and v1.0.x)

Used internally for testing and limited deployment. Not available to the public.

---

Have feedback or ideas? [Join the Discord Support Server](https://discord.gg/fxhXWgxcHV)

---

[← Back to Readme](README.md)
