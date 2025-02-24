# HawkWatch Bot Command Usage

![hawkwatch banner image](/images/hawk_banner.jpg)

- [HawkWatch Bot Command Usage](#hawkwatch-bot-command-usage)
    - [Required Permissions](#required-permissions)
        - [Bot Permissions](#bot-permissions)
        - [User Requirements](#user-requirements)
    - [Quick Start](#quick-start)
    - [Game Tracking Commands](#game-tracking-commands)
        - [Track a Game for Updates](#track-a-game-for-updates)
        - [Stop Tracking a Game for Updates](#stop-tracking-a-game-for-updates)
        - [List Watched Games](#list-watched-games)
        - [Set Watch Settings](#set-watch-settings)
        - [Get Watch Settings](#get-watch-settings)
    - [Search Commands](#search-commands)
        - [Search](#search)
    - [About HawkWatch](#about-hawkwatch)
        - [Features:](#features)
        - [Need more help?](#need-more-help)
        - [Developer:](#developer)



## Required Permissions

### Bot Permissions

HawkWatch requires the following permissions to function properly:
- **View Channel**: Allow me to see the channel, but not its messages.
- **Send Messages**: Allow me to send messages in the channel.
- **Send Messages in Threads**: Allow me to send messages in threads.
- **Embed Links**: Allow me to send embeds in the channel (they look pretty).

### User Requirements

HawkWatch commands can only be used by:

- Server Owner
- Server Administrators
- Users with role `mod` or `admin`

---

## Quick Start
- **Track a game:** `/watch game name:<name|id>`
- **Stop tracking:** `/unwatch name:<name|id>`
- **List watched games:** `/list watched`

---

## Game Tracking Commands

### `Track a Game for Updates`
**Description:**
Start tracking updates for a game by name or ID.

Only channel types of **Text** or **Thread** (public or private) are supported.

Note that you can only track 2 games at a time, this may change in the future.

**Usage:**

```
/watch game name:<name|id> notify:<channel>
```

**Options:**
- **name** (*String/Integer*, Required) - Name or Game ID of the game to track.
- **notify** (*Channel Name*, Default: Current Channel) - Specify a channel to send updates to.

**Examples:**
- **/watch game name:RIVALS** - Start tracking updates for the game 'RIVALS' in the current channel.
- **/watch game name:17625359962** - Start tracking updates for the game with ID '17625359962' in the current channel.
- **/watch game name:RIVALS notify:updates** - Send updates to the channel 'updates' for game RIVALS.

---

### `Stop Tracking a Game for Updates`
**Description:**
Stop tracking a game.

Please be aware that unwatching a game prevents you from adding a new game for 24hrs! If it was a mistake you can immediately rewatch the game just removed.

**Usage:**

```
/unwatch name:<name|id>
```

**Options:**
- **name** (*String/Integer*, Required) - Name or Game ID of the game to untrack.

**Examples:**
- **/unwatch name:RIVALS** - Stop tracking the game 'RIVALS'.
- **/unwatch name:17625359962** - Stop tracking the game with ID '17625359962'.

---

### `List Watched Games`
**Description:**
List all games currently being tracked.

**Usage:**

```
/list watched
```

**Options:**
- **Post** (*True/False*, Default: False) - If you want to post the message so others can see results.

---

### `Set Watch Settings`
**Description:**
Configure tracking options for a game.

**Usage:**

```
/watch settings set game_name:<name|id> [options]
```

**Options:**

- **channel** (*Channel Name/Empty*, Default: Unchanged) - Specify a channel to send updates to.
- **date** (*Track / Don't Track / Empty*, Default: Track) - Enable/disable alerting when the game's date changes.
- **thumbnail** (*Track / Don't Track / Empty*, Default: Track) - Enable/disable alerting when the game's thumbnail(s) change.
- **name** (*Track / Don't Track / Empty*, Default: Track) - Enable/disable alerting when the game's name changes.
- **description** (*Track / Don't Track / Empty*, Default: Track) - Enable/disable alerting when the game's description changes.

**Examples:**
- **/watch settings set game_name:Brookhaven 🏡RP channel:updates** - Set the tracking channel for game Brookhaven 🏡RP.
- **/watch settings set game_name:4924922222 thumbnail:Don't Track** - Disable thumbnail tracking for the game with ID '4924922222'.
- **/watch settings set game_name:Brookhaven 🏡RP** - Keep all options at their defaults.
- **/watch settings set game_name:Brookhaven 🏡RP date:Don't Track name:Don't Track** - Disable tracking for date and name changes.

---

### `Get Watch Settings`
**Description:**
View current tracking settings for a game.

**Usage:**

```
/watch settings get game_name:<name>
```

**Options:**
- **name** (*String/Integer*, Required) - Name or Game ID of the game to view settings for.

**Examples:**
- **/watch settings get game_name:Brookhaven 🏡RP** - View tracking settings for the game 'Brookhaven 🏡RP'.
- **/watch settings get game_name:17625359962** - View tracking settings for the game with ID '17625359962'.

---

## Search Commands

### `Search`
**Description:**
Search for a game by name, creator, or genre. At least one option is required. Partial values are accepted.

**Usage:**

```
/search <name|creator|genre>
```

**Options:**
- **name** (*String*, Default: None) - Search for a game by name.
- **creator** (*String*, Default: None) - Search for a game by creator.
- **genre** (*String*, Default: None) - Search for a game by genre.

**Examples:**
- **/search name:RIVALS** - Search for a game with the name 'RIVALS'.
- **/search creator:Shedletsky** - Search for games created by 'Shedletsky'.
- **/search genre:FPS** - Search for games in the 'FPS' genre.
- **/search name:RIVALS creator:Shedletsky** - Search for games with the name 'RIVALS' created by 'Shedletsky'.

---

## About HawkWatch
This bot is designed to help you track and manage which updates for Roblox games you receive.

### Features:
- Get live notifications for game updates. Currently limited to watching 2 games (this may change in the future).
- Search for games by name, creator, or genre. Note that search details only update ~30 days and are not kept current!

### Need more help?
Join our support server: [Click Here to Join](https://discord.gg/f6RYDdu9ms) and head to the support channel to submit a bug report or feature request.

### Developer:

**BloominDaisy**
