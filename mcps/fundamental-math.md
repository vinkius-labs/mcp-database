# Fundamental Math MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fundamental-math)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

A deterministic, zero-latency mathematical engine for exact calculations. Safely compute percentages, square roots, factorials, and the rule of three completely local.

## Description
Large Language Models are brilliant at reasoning, but they notoriously hallucinate when performing exact mathematics. The Fundamental Math MCP Server solves this by providing your autonomous agents with a deterministic, zero-latency computational engine.

### The Superpowers
- **Zero Hallucinations:** Guarantees 100% mathematical accuracy for critical workflows like finance and statistics.
- **Privacy First (Local):** Executes purely in local JavaScript. No API calls, no data leaves your secure enclave.
- **The Classic Rule of Three:** Easily solve proportional problems (if A is to B, then C is to X) without complex prompting.
- **Essential Toolkit:** Built-in tools for percentages, square roots, exponential powers, and factorials.

Stop relying on probabilistic models for exact numbers. Equip your agent with a real calculator.


## Available Tools
- **calculate_factorial**: Calculates the factorial of a non-negative integer
- **calculate_percentage**: Calculates the percentage of a given total value
- **calculate_power**: Calculates the base raised to the exponent power
- **calculate_rule_of_three**: Solves a simple rule of three (proportionality)
- **calculate_square_root**: Calculates the square root of a given number


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fundamental Math** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a total budget of 4500 and I want to allocate 17.5% to marketing. Calculate the exact value."

**🤖 AI Agent:**
> Using the calculate_percentage tool: The exact value for 17.5% of 4500 is 787.5.

---

**👤 You:**
> "If an ad campaign generated 120 leads with a $500 investment, how many leads can I expect with a $2500 investment?"

**🤖 AI Agent:**
> Using the calculate_rule_of_three tool (A=500, B=120, C=2500): You can expect exactly 600 leads with a $2500 investment.

---

**👤 You:**
> "Calculate the factorial of 12 for my probability distribution script."

**🤖 AI Agent:**
> Using the calculate_factorial tool: The factorial of 12 (12!) is exactly 479,001,600.


## ❓ FAQ

**Q: Why use this instead of asking the AI to calculate it?**
AI models predict the next token; they don't actually compute math. This leads to subtle and dangerous errors in calculations. This MCP forces the AI to use a deterministic JavaScript engine, ensuring absolute precision.

**Q: Does this server require an internet connection or an external API?**
Absolutely not. It is built entirely on pure, local JavaScript logic. It requires zero configuration, zero API keys, and guarantees that your sensitive data never leaves your infrastructure.

**Q: How does the 'Rule of Three' tool work?**
The Rule of Three tool solves proportional logic instantly. If you know that 100 units cost $50, you can pass A=100, B=50, and C=250 to find exactly how much 250 units will cost. The agent will handle the correlation automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fundamental-math](https://vinkius.com/mcp/fundamental-math)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fundamental Math** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fundamental-math` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fundamental Math** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fundamental-math": {
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
