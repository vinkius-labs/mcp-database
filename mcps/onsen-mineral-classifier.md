# Onsen Mineral Classifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/onsen-mineral-classifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Classify Japanese hot spring water quality, legal status, and therapeutic benefits.

## Description
This MCP server provides deterministic tools for analyzing Japanese hot spring (Onsen) water. It determines if water meets legal Onsen definitions using `validate_onsen_status`, evaluates health benefits via `calculate_therapeutic_profile`, predicts cooling times with `estimate_cooling_duration`, and monitors safety using `check_ph_safety`.


## Available Tools (4)
- **calculate_therapeutic_profile**: Evaluates the skin and health benefits provided by the specific mineral composition
- **estimate_cooling_duration**: Predicts how long it takes for the water to reach a safe bathing temperature
- **validate_onsen_status**: Determines if the water meets the legal definition of an Onsen
- **check_ph_safety**: Flags extreme pH levels that require safety warnings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Onsen Mineral Classifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a spring with 26°C water and sulfur content a legal Onsen?"

**🤖 AI Agent:**
> Yes, it is a valid Onsen because the temperature is 25°C or higher.

---

**👤 You:**
> "What are the benefits of sulfur-rich water?"

**🤖 AI Agent:**
> Sulfur is highly beneficial for treating skin conditions like dermatitis.

---

**👤 You:**
> "How long until 50°C water reaches 40°C if the air is 20°C?"

**🤖 AI Agent:**
> The water will reach the target temperature in approximately 45 minutes.


## ❓ FAQ

**Q: How do I check if a spring is legally an Onsen?**
Use the `validate_onsen_status` tool by providing the water temperature and the dominant mineral type.

**Q: Can I calculate how long it takes for water to cool down?**
Yes, the `estimate_cooling_duration` tool predicts the time needed to reach a safe bathing temperature based on initial and ambient temperatures.

**Q: How is water safety checked?**
The `check_ph_safety` tool flags extreme pH levels that require dilution warnings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/onsen-mineral-classifier](https://vinkius.com/ai-agent-connect/onsen-mineral-classifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Onsen Mineral Classifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `onsen-mineral-classifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Onsen Mineral Classifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "onsen-mineral-classifier": {
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
