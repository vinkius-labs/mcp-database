# Rug Pull Detection Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/rug-pull-detection-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Identify high-risk tokens by analyzing liquidity locks, contract privileges, and holder distribution.

## Description
This MCP server provides a deterministic risk assessment engine to protect traders from liquidity removal and developer exit scams. By connecting your AI client to Vinkius Edge, you can use tools like `analyze_token_risk` to evaluate a token's security profile. The engine calculates a rug risk score based on critical factors: liquidity lock percentage, owner minting privileges, top holder concentration, and transaction limits. It also identifies honeypots and calculates liquidity removal risk. This allows agents to provide clear trading recommendations--Safe, Caution, or Avoid--before capital is committed.


## Available Tools (3)
- **analyze_token_risk**: Provides a comprehensive risk profile and a final trading recommendation for a specific token
- **get_holder_metrics**: Evaluates the distribution of token ownership to identify centralization risks
- **get_liquidity_status**: Checks the current state of liquidity to determine if it is sufficient and how much is committed to the protocol


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rug Pull Detection Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the risk for token address 0x1234567890abcdef1234567890abcdef12345678 with $150,000 liquidity."

**🤖 AI Agent:**
> The token has a rug risk score of 25. With 80% liquidity locked and no minting privileges, the recommendation is SAFE.

---

**👤 You:**
> "Check if this token is a honeypot: 0xabc123..."

**🤖 AI Agent:**
> The contract analysis shows the honeypot flag is true, meaning the contract prevents selling. Recommendation: AVOID.

---

**👤 You:**
> "What is the holder concentration for the token at 0xdef456...?"

**🤖 AI Agent:**
> The top 10 holders control 65% of the total supply, indicating high centralization risk.


## ❓ FAQ

**Q: How is the rug risk score calculated?**
The score is a weighted sum of penalties: low liquidity locks, owner minting rights, high holder concentration, lack of transaction limits, and low liquidity depth.

**Q: What does a 'CAUTION' recommendation mean?**
A CAUTION recommendation indicates a moderate risk score that does not meet the threshold for an immediate AVOID, but requires careful scrutiny of the contract.

**Q: Can I use this with Claude Desktop?**
Yes, you can connect this MCP to Claude Desktop, Cursor, VS Code, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/rug-pull-detection-strategy](https://vinkius.com/ai-agent-connect/rug-pull-detection-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rug Pull Detection Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rug-pull-detection-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rug Pull Detection Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rug-pull-detection-strategy": {
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
