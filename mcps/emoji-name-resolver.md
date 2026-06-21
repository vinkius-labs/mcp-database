# Emoji Name Resolver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emoji-name-resolver)
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


## Available Tools (1)
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


## ❓ FAQ

**Q: How many emojis are supported?**
Over 1,800 emojis from the Unicode standard, including all standard shortcodes used by Slack, Discord, and GitHub.

**Q: Can it process full sentences with multiple emojis?**
Yes. Pass a full message like 'Great job :thumbsup: keep going :rocket:' and it will convert all shortcodes in one call.

**Q: What shortcode format does it use?**
The standard colon-wrapped format used by Slack, Discord, and GitHub: `:emoji_name:`. For example, `:fire:`, `:heart:`, `:rocket:`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emoji-name-resolver](https://vinkius.com/mcp/emoji-name-resolver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emoji Name Resolver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emoji-name-resolver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emoji Name Resolver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emoji-name-resolver": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
