# Darts Checkout Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/darts-checkout-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [games](../categories/games.md)

A deterministic engine for calculating valid darts checkout combinations and optimal paths.

## Description
This MCP server provides a deterministic engine for professional darts scoring (501/301). It calculates all valid checkout combinations, identifies the most efficient paths using high-value triples, and manages bust logic. Use `get_valid_checkouts` to see all possible ways to finish, `get_optimal_checkout` to find the best path, and `validate_shot_legality` to check if a throw resulted in a bust or a successful finish.


## Available Tools (3)
- **get_optimal_checkout**: Identifies the single most efficient dart sequence to complete the checkout
- **get_valid_checkouts**: Retrieves all possible dart combinations that successfully reach zero from the current score
- **validate_shot_legality**: Checks if a specific dart or sequence of darts results in a bust or an invalid state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Darts Checkout Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the ways to checkout 170 in 3 darts?"

**🤖 AI Agent:**
> The valid combination for 170 is T20-T20-Bull.

---

**👤 You:**
> "What is the best way to finish 100?"

**🤖 AI Agent:**
> The optimal checkout for 100 is T20-D20.

---

**👤 You:**
> "I have 40 left and I hit a single 20. Did I bust?"

**🤖 AI Agent:**
> No, you have 20 remaining and the game is still in progress.


## ❓ FAQ

**Q: What is a 'bust' in darts?**
A bust occurs if the thrown darts reduce the score to below zero or to exactly one, as a checkout must end on a double or bullseye.

**Q: How do I find the best way to finish a score?**
You can use the `get_optimal_checkout` tool to identify the most efficient sequence, which prioritizes high-value triples to leave preferred doubles.

**Q: Can I check if my last throw was valid?**
Yes, use `validate_shot_legality` to determine if your darts resulted in a bust, a zero score, or if the game is still in progress.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/darts-checkout-calculator](https://vinkius.com/ai-agent-connect/darts-checkout-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Darts Checkout Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `darts-checkout-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Darts Checkout Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "darts-checkout-calculator": {
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
