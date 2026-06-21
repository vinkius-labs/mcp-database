# Emoji Name Resolver MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emoji-name-resolver)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/emoji-name-resolver-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/emoji-name-resolver-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert emoji shortcodes to Unicode and back (:rocket: ↔ 🚀). Essential for Slack, Discord, and GitHub cross-platform compatibility.

## Description
When a Martech agent crafts messages for Slack, Discord, and GitHub, each platform uses different emoji formats. This MCP resolves bidirectionally with a database of 1,800+ emojis.

### The Superpowers

- **Bidirectional:** `:rocket:` → `🚀` and `🚀` → `:rocket:`.
- **Full String Support:** Processes entire messages, not just single emojis.
- **1,800+ Emojis:** Complete database covering all standard Unicode emojis.


## Available Tools
- **resolve_emoji**: Pass the input text and direction ("name-to-emoji" to convert :shortcodes: to emojis, or "emoji-to-name" to convert emojis back to :shortcodes:). Works on full strings with multiple emojis.

Converts emoji shortcodes to Unicode emojis (:rocket: -> 🚀) and vice versa (🚀 -> :rocket:). Essential for cross-platform compatibility between Slack, Discord, and GitHub


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emoji Name Resolver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert :rocket: :fire: :star: to actual emojis."

**🤖 AI Agent:**
> Result: 🚀 🔥 ⭐

---

**👤 You:**
> "What are the shortcode names for 🎉👍💯?"

**🤖 AI Agent:**
> Result: :tada: :thumbsup: :100:

---

**👤 You:**
> "Emojify this Slack message: 'Deploy successful :white_check_mark: zero downtime :muscle:'"

**🤖 AI Agent:**
> Result: Deploy successful ✅ zero downtime 💪


## Installation & Usage

To install and use the **Emoji Name Resolver** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emoji-name-resolver](https://vinkius.com/mcp/emoji-name-resolver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
