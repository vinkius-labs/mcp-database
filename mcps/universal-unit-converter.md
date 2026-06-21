# Universal Unit Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/universal-unit-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A zero-latency deterministic engine for exact physical conversions. Instantly convert weights, lengths, temperatures, and digital storage local.

## Description
Large Language Models often approximate metric-to-imperial conversions, which can lead to critical errors in engineering, development, or logistics. The Universal Unit Converter MCP delegates these conversions to a robust, exact mathematical engine.

### The Superpowers
- **Zero Approximation:** Guarantees absolute mathematical precision by replacing LLM guesses with deterministic JavaScript algorithms.
- **Universal Coverage:** Flawlessly converts across Length (metric/imperial), Weight, Temperature (C/F/K), and Digital Storage (using binary 1024 multipliers).
- **Privacy First (Local):** Executes 100% locally. Zero API calls, meaning your sensitive engineering metrics or server logs never leave your machine.


## Available Tools (4)
- **convert_digital_storage**: g., 1 KB = 1024 B).

Converts digital storage using binary prefixes (B, KB, MB, GB, TB)
- **convert_length**: Converts length between metric and imperial (km, m, cm, mm, mi, yd, ft, in)
- **convert_temperature**: Converts temperature between Celsius (C), Fahrenheit (F), and Kelvin (K)
- **convert_weight**: Converts weight between metric and imperial (kg, g, lb, oz)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Universal Unit Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert 135 pounds (lb) to kilograms."

**🤖 AI Agent:**
> Using the convert_weight tool: 135 lb is exactly 61.2350 kg.

---

**👤 You:**
> "If a server requires 8192 MB of RAM, how many GB is that?"

**🤖 AI Agent:**
> Using the convert_digital_storage tool: 8192 MB is exactly 8 GB.

---

**👤 You:**
> "Convert 78 degrees Fahrenheit to Celsius for the weather report."

**🤖 AI Agent:**
> Using the convert_temperature tool: 78 F is 25.56 C.


## ❓ FAQ

**Q: Are digital storage conversions based on base-10 (1000) or base-2 (1024)?**
The digital storage tool strictly uses base-2 (binary multipliers of 1024), which is the standard for memory and file system operations (e.g., 1 KB = 1024 B).

**Q: Why use this instead of letting Claude or ChatGPT convert the values?**
LLMs hallucinate subtle decimal errors when converting odd metrics (like 17.3 miles to centimeters). This tool forces the AI to use exact deterministic formulas.

**Q: Does it require internet access?**
No. The entire engine is local and executes purely on local hardware without any API requests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/universal-unit-converter](https://vinkius.com/mcp/universal-unit-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Universal Unit Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `universal-unit-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Universal Unit Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "universal-unit-converter": {
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
