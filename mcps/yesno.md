# YesNo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yesno)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Get instant yes, no, or maybe decisions accompanied by fun GIFs to help your AI agent make choices or break ties.

## Description
Connect to the **YesNo.wtf** API to bring a touch of randomness and visual flair to your AI interactions. Whether you need to settle a debate, make a quick choice, or just add some fun to a conversation, this server provides definitive answers with matching animated GIFs.

### What you can do

- **Random Decisions** — Get a "yes", "no", or "maybe" answer instantly from the API.
- **Visual Feedback** — Every decision comes with a relevant GIF URL to visualize the response in your chat interface.
- **Forced Answers** — Use the optional force parameter to get a specific outcome (yes/no/maybe) while still receiving a corresponding GIF.
- **Tie-Breaking** — Use the agent as a neutral third party to make binary or ternary choices.

### How it works

1. Subscribe to this server
2. No API key is required for this public service
3. Start asking your agent to make decisions using the YesNo tool

### Who is this for?

- **Developers** — add a fun, interactive element to bot responses or testing workflows.
- **Casual Users** — use the AI to help make trivial daily choices with a visual twist.
- **Content Creators** — generate quick visual reactions based on random or forced logic.


## Available Tools
- **get_decision**: Can optionally force a specific answer.

Get a random yes/no/maybe decision with a GIF


## 💬 Prompt Examples

Here are some examples of how you can interact with the **YesNo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Should I have another cup of coffee? Ask YesNo."

**🤖 AI Agent:**
> I've consulted the oracle... The answer is 'yes'! Here is a GIF to celebrate your next caffeine boost: [GIF URL]

---

**👤 You:**
> "Give me a 'maybe' decision with a GIF."

**🤖 AI Agent:**
> Forcing a 'maybe' decision for you... The result is 'maybe'. Check out this GIF: [GIF URL]

---

**👤 You:**
> "I can't decide if I should go for a run. Get a random decision."

**🤖 AI Agent:**
> The universe has spoken: 'no'. Maybe stay in and relax? Here's a GIF reflecting that choice: [GIF URL]


## ❓ FAQ

**Q: Can I force the tool to return a specific answer like 'yes'?**
Yes! The `get_decision` tool includes an optional `force` parameter. You can specify 'yes', 'no', or 'maybe' to get that exact answer along with a corresponding GIF.

**Q: Does the response always include a GIF?**
Every successful call to `get_decision` returns a JSON object containing the answer string and a direct URL to an animated GIF from the YesNo.wtf library.

**Q: Is an API key required to use this server?**
No. This server connects to the public YesNo.wtf API which does not require authentication. You can start using it immediately after subscribing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yesno](https://vinkius.com/mcp/yesno)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **YesNo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `yesno` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **YesNo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yesno": {
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
