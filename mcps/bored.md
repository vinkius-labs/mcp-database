# Bored MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bored)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Find the perfect activity to beat boredom — filter by category, participants, price, and accessibility directly from your AI agent.

## Description
Connect the **Bored API** to your AI agent and never run out of things to do. Whether you are looking for a solo DIY project or a social activity for a large group, this server helps you discover curated suggestions through natural conversation.

### What you can do

- **Random Discovery** — Get a completely random activity suggestion instantly when you don't know where to start.
- **Targeted Search** — Filter activities by type (education, social, relaxation, etc.), number of participants, or specific price ranges.
- **Accessibility Mapping** — Find tasks that match your physical or situational constraints using accessibility scores.
- **Specific Retrieval** — Use unique keys to pull up specific activities you've seen before or want to reference.

### How it works

1. Subscribe to this server
2. Configure your access (no complex setup required)
3. Ask your AI for suggestions based on your current mood or group size

### Who is this for?

- **Individuals** — looking for quick ways to learn something new or relax.
- **Event Organizers** — searching for social or recreational ideas for specific group sizes.
- **Developers** — testing agent capabilities with a clean, structured data source for suggestions.


## Available Tools (3)
- **get_activity_by_key**: Get a specific activity by its unique key
- **find_activity**: Find an activity based on specific criteria
- **get_random_activity**: Get a random activity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bored** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm bored, give me a random activity to do."

**🤖 AI Agent:**
> How about this: 'Learn how to juggle'. It's a recreational activity that requires 1 participant and has an accessibility score of 0.3.

---

**👤 You:**
> "Find a social activity for 4 people that is free."

**🤖 AI Agent:**
> I found a great suggestion: 'Play a game of ultimate frisbee'. It's categorized as social, supports 4 participants, and costs 0.0.

---

**👤 You:**
> "What are the details for activity key 5881028?"

**🤖 AI Agent:**
> Activity 5881028 is 'Learn a new cooking recipe'. It's a cooking type activity for 1 person with a price point of 0.2 and high accessibility.


## ❓ FAQ

**Q: Can I find activities specifically for a large group of people?**
Yes! You can use the `find_activity` tool and specify the `participants` parameter to get suggestions tailored to your group size.

**Q: How do I search for activities that are completely free?**
Simply use the `find_activity` tool and set the `price` parameter to 0.0. You can also use `maxprice` to set a budget limit.

**Q: Can I retrieve an activity if I only have its ID number?**
Absolutely. Use the `get_activity_by_key` tool and provide the unique numeric key to fetch the full details of that specific activity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bored](https://vinkius.com/mcp/bored)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bored** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bored` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bored** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bored": {
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
