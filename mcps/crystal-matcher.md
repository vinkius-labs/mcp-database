# Crystal Matcher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crystal-matcher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [wellness](../categories/wellness.md)

Connect AI agents to a curated catalog of crystals based on intent, element, and chakra.

## Description
## Connect AI Agents to the Crystal Matcher Catalog

Finding the right crystal for a specific intention can be complex. Whether you are seeking protection, love, abundance, or healing, matching your energetic needs with the correct stone requires knowledge of properties, elements, and chakras.

This MCP server gives AI agents direct access to an extensive catalog of over 80 crystals through tools like `query_crystals_by_intent`, `get_crystal_details`, `filter_crystals_by_element`, and `find_crystals_by_chakra`. Agents can interpret a user's spiritual or emotional goal and return precise recommendations based on vibrational matching.

Instead of manual searching, ask your AI assistant: *"Which crystals are good for the Heart chakra?"* The agent calls `find_crystals_by_chakra`, retrieves the list, and presents the associated stones and their properties.

Connects through Vinkius Edge -- one URL, one token, no API keys to manage.


## Available Tools (4)
- **get_crystal_details**: Get detailed information about a specific crystal
- **filter_crystals_by_element**: Filter crystals by their associated element
- **find_crystals_by_chakra**: Find crystals associated with a specific chakra
- **query_crystals_by_intent**: Find crystals based on a spiritual or emotional intent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crystal Matcher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am feeling very anxious and need grounding. Which crystals should I use?"

**🤖 AI Agent:**
> To help with grounding and anxiety, I recommend looking into stones associated with the Earth element or the Root chakra. Based on your need for grounding, you might consider using Black Tourmaline or Hematite, which are known for their stabilizing properties.

---

**👤 You:**
> "List all crystals associated with the Heart chakra."

**🤖 AI Agent:**
> I found several crystals for the Heart chakra, including Rose Quartz, Jade, and Emerald. These stones are primarily used to promote love, compassion, and emotional healing.

---

**👤 You:**
> "Tell me more about the properties of Amethyst."

**🤖 AI Agent:**
> **Amethyst**

- **Properties**: Calm, Clarity, Protection
- **Element**: Air
- **Chakra**: Third Eye

Amethyst is a powerful stone for spiritual protection and enhancing intuition.


## ❓ FAQ

**Q: How can an agent find crystals for a specific need?**
Agents use the `query_crystals_by_intent` tool. By providing an intent like 'protection' or 'abundance', the agent retrieves crystals whose properties align with that goal.

**Q: Can I search for crystals by their element?**
Yes. Using `filter_crystals_by_element`, an agent can find all stones associated with Earth, Air, Fire, Water, or Ether.

**Q: Does this require a subscription to a crystal database?**
No. The catalog is built into the MCP server itself, providing instant access via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crystal-matcher](https://vinkius.com/mcp/crystal-matcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crystal Matcher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crystal-matcher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crystal Matcher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crystal-matcher": {
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
