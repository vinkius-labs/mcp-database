# MEV Sandwich Detection Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mev-sandwich-detection-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Identify and avoid sandwich attacks in DEX transactions.

## Description
This MCP server provides tools to detect and analyze Maximal Extractable Value (MEV) sandwich attacks. Use `detect_sandwich_pattern` to determine if a specific transaction was targeted by front-running and back-running bots. Use `analyze_sandwich_statistics` to get aggregate data on attack frequency and affected tokens. Use `evaluate_protection_strategy` to receive risk assessments and recommendations for specific trades to minimize slippage and avoid high-risk tokens.


## Available Tools (3)
- **detect_sandwich_pattern**: Determines if a specific transaction was the victim of a sandwich attack pattern
- **analyze_sandwich_statistics**: Provides high-level aggregate metrics regarding the frequency and intensity of sandwich attacks
- **evaluate_protection_strategy**: Evaluates whether a specific token or trade should be avoided based on current MEV risk levels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MEV Sandwich Detection Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Was this transaction sandwiched?"

**🤖 AI Agent:**
> The transaction was indeed part of a sandwich attack, resulting in a victim impact of 4.5%.

---

**👤 You:**
> "Should I trade this token?"

**🤖 AI Agent:**
> No, you should avoid this token as its sandwich frequency is currently above 5%.

---

**👤 You:**
> "What is the current sandwich attack frequency?"

**🤖 AI Agent:**
> The current sandwich frequency is 12 attacks per 1000 DEX transactions.


## ❓ FAQ

**Q: How do I know if a transaction was a sandwich attack?**
You can use the `detect_sandwich_pattern` tool with your transaction and mempool data to confirm if a sandwich pattern occurred.

**Q: Can this tool help me avoid MEV?**
Yes, `evaluate_protection_strategy` provides specific advice, such as adjusting slippage tolerance or using private RPCs, to mitigate risk.

**Q: What metrics does the statistics tool provide?**
The `analyze_sandwich_statistics` tool returns the frequency of attacks per 1000 transactions, average profit per attack, and a list of most affected tokens.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mev-sandwich-detection-strategy](https://vinkius.com/ai-agent-connect/mev-sandwich-detection-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MEV Sandwich Detection Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mev-sandwich-detection-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MEV Sandwich Detection Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mev-sandwich-detection-strategy": {
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
