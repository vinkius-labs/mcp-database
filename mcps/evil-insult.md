# Evil Insult MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/evil-insult)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate creative and random insults from the Evil Insult Generator API directly within your AI agent.

## Description
Add a touch of "evil" humor to your workflows. This MCP server connects to the **Evil Insult Generator**, allowing your AI to fetch and deliver randomized insults in multiple languages.

### What you can do

- **Random Generation** — Fetch a unique, randomized insult instantly.
- **Multi-language Support** — Get insults in English, Spanish, French, Russian, German, and more.
- **Creative Writing** — Use generated insults for character dialogue, testing, or just for fun.

### How it works

1. Subscribe to this server
2. No complex API keys are required for basic access
3. Use the `generate_insult` tool to start the roasting

### Who is this for?

- **Developers** — Add humorous placeholders or test data to applications.
- **Gamers & Creators** — Spice up community interactions or character scripts.
- **Anyone** — Who needs a quick, sharp comeback provided by an AI.


## Available Tools
- **generate_insult**: You can optionally specify a language code.

Generate an evil insult


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Evil Insult** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a random insult."

**🤖 AI Agent:**
> I've fetched an insult for you: 'You are so slow, the birds use you as a landmark.'

---

**👤 You:**
> "Give me an insult in Spanish."

**🤖 AI Agent:**
> Using the Spanish generator: '¡Eres más inútil que el primer capítulo de los Power Rangers!'

---

**👤 You:**
> "Generate an insult in French using the generate_insult tool."

**🤖 AI Agent:**
> Executing generate_insult for French... Result: 'Tu es tellement moche que même les aveugles ferment les yeux.'


## ❓ FAQ

**Q: Can I choose the language of the insult?**
Yes! Use the `generate_insult` tool and provide a language code like 'en', 'es', 'fr', 'ru', or 'de' in the `lang` parameter.

**Q: Where do these insults come from?**
All insults are fetched in real-time from the official Evil Insult Generator API.

**Q: Is there a limit to how many insults I can generate?**
The tool generates one insult per request. You can call the `generate_insult` tool as many times as you need to get fresh results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/evil-insult](https://vinkius.com/mcp/evil-insult)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Evil Insult** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `evil-insult` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Evil Insult** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "evil-insult": {
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
