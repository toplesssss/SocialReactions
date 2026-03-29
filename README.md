# Social Reactions

**Express emotions instantly – react to other players with visual effects and sounds!**

[![Paper](https://img.shields.io/badge/Paper-1.20+-blue?logo=paper)](https://papermc.io/)
[![Java](https://img.shields.io/badge/Java-21-orange)](https://adoptium.net/)
[![Version](https://img.shields.io/badge/version-1.0-brightgreen)](https://github.com/yourusername/SocialReactions/releases)

## 🎭 What is Social Reactions?

**Social Reactions** is a lightweight Minecraft plugin that lets players react to each other with emotions – applause, sympathy, anger, fear, celebration, and disapproval. All reactions are visible as **particle effects** and **sounds** above the target player, creating immersive roleplay moments **without adding a single item or block**.

Perfect for **SMP**, **Roleplay**, and **vanilla‑style** servers.

---

## ✨ Features

- ✅ **6 reaction types** – praise, sympathy, anger, fear, celebrate, disapprove
- 🎨 **Visual particles** – each reaction has a unique particle effect (hearts, flames, smoke, etc.)
- 🔊 **Sound effects** – applause, sigh, angry grunt, gasp, cheers, boos
- 🌍 **Multilingual** – built‑in English and Russian. Easily add your own language
- 📊 **Optional reputation** – reactions can affect player reputation (fully configurable)
- ⚙️ **Fully configurable** – cooldowns, range, messages, effect durations
- ✅ **No new items or blocks** – pure vanilla‑friendly
- 📈 **PlaceholderAPI** support – track your stats

---

## 📦 Commands

| Command | Description | Permission |
|---------|-------------|------------|
| `/react <player> <type>` | React to a player | `socialreactions.use` |
| `/reputation` | Check your reputation | `socialreactions.use` |
| `/socialreactions reload` | Reload configuration | `socialreactions.admin` |

**Reaction types:** `praise`, `sympathy`, `anger`, `fear`, `celebrate`, `disapprove`

---

## 🔧 Installation

1. Download `SocialReactions-1.0.jar` from the [Releases](https://github.com/yourusername/SocialReactions/releases) page.
2. Place it in your server's `plugins/` folder.
3. Restart your server.
4. Edit `config.yml` to your liking (cooldowns, language, reputation values).
5. (Optional) Set `language: ru` in config for Russian.

---

## ⚙️ Configuration

```yaml
language: en

reactions:
  cooldown-seconds: 10
  range: 20
  reputation-impact: true
  reputation-values:
    praise: 1
    sympathy: 1
    anger: -1
    fear: 0
    celebrate: 1
    disapprove: -1

particles:
  praise: HEART
  sympathy: CLOUD
  anger: FLAME
  fear: SMOKE
  celebrate: FIREWORK
  disapprove: CAMPFIRE_COSY_SMOKE

sounds:
  praise: ENTITY_PLAYER_LEVELUP
  sympathy: ENTITY_PLAYER_SIGH
  anger: ENTITY_IRON_GOLEM_HURT
  fear: ENTITY_PLAYER_HURT
  celebrate: ENTITY_PLAYER_CHEER
  disapprove: ENTITY_PLAYER_BURP

```

🌍 Languages
English – lang/en.yml

Russian – lang/ru.yml

To add your own language, copy en.yml to lang/yourlang.yml, translate the values, and set language: yourlang in config.yml.

---

📊 PlaceholderAPI
If PlaceholderAPI is installed, you can use:

%socialreactions_reputation% – current reputation score

%socialreactions_used_total% – total reactions you've given

%socialreactions_received_total% – total reactions you've received

---
Made with ❤️ by Toples
