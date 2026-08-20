# Sake Seimai Buai Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sake-seimai-buai-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate rice milling yields, milling duration, sake grades, and fermentation water requirements.

## Description
This MCP server provides deterministic calculations for Japanese sake production. It allows AI agents to determine the exact weight of polished rice using `calculate_milling_yield`, estimate processing time with `estimate_milling_duration`, identify premium sake classifications via `classify_sake_grade`, and determine brewing needs with `calculate_fermentation_water`.


## Available Tools (4)
- **calculate_fermentation_water**: Calculates the required water mass for fermentation based on the polished rice weight
- **calculate_milling_yield**: Determines the resulting weight of polished rice and the amount of bran removed
- **estimate_milling_duration**: Calculates how long the milling process will take based on the volume of material being removed
- **classify_sake_grade**: Determines the premium classification of the sake based on the target polishing ratio


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sake Seimai Buai Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 100kg of brown rice and want a 50% polishing ratio. How much polished rice will I have?"

**🤖 AI Agent:**
> You will have 50kg of polished rice.

---

**👤 You:**
> "What sake grade is a 55% polishing ratio?"

**🤖 AI Agent:**
> A 55% polishing ratio is classified as Ginjo.

---

**👤 You:**
> "How much water do I need for 50kg of polished rice if the ratio is 1.3?"

**🤖 AI Agent:**
> You will need 65kg of water.


## ❓ FAQ

**Q: How do I determine the sake grade?**
You can use the `classify_sake_grade` tool to find the classification based on the target polishing ratio.

**Q: Can I calculate how much bran (nuka) is removed?**
Yes, the `calculate_milling_yield` tool returns both the polished rice weight and the weight of the nuka removed.

**Q: How is milling time calculated?**
The `estimate_milling_duration` tool calculates the time by dividing the weight of the removed nuka by the machine's milling rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sake-seimai-buai-calculator](https://vinkius.com/ai-agent-connect/sake-seimai-buai-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sake Seimai Buai Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sake-seimai-buai-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sake Seimai Buai Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sake-seimai-buai-calculator": {
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
