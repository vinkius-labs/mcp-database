# UV Exposure Risk Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/uv-exposure-risk-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Estimate sunburn risk, safe sun exposure time, and Vitamin D synthesis potential.

## Description
This MCP server provides tools to calculate skin safety during UV exposure. Use `calculate_sunburn_risk` to determine the likelihood of redness, `get_safe_exposure_window` to find how many minutes you can safely stay in the sun, and `estimate_vitamin_d_potential` to assess Vitamin D synthesis. It also includes `compare_protection_efficacy` to evaluate different SPF levels.


## Available Tools (4)
- **calculate_sunburn_risk**: Determines the likelihood of skin redness for a specific exposure session
- **compare_protection_efficacy**: Evaluates how much a specific SPF increases the user's window of safety
- **estimate_vitamin_d_potential**: Assesses the ability to synthesize Vitamin D during the current conditions
- **get_safe_exposure_window**: Calculates how long a user can safely stay in the sun before reaching the redness threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UV Exposure Risk Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my sunburn risk if I stay in the sun for 20 minutes with a UV index of 8 and skin type II using SPF 30?"

**🤖 AI Agent:**
> Your risk level is Low, and your estimated erythema threshold is significantly extended by the SPF 30.

---

**👤 You:**
> "How many minutes can I safely stay in the sun with a UV index of 5 and skin type III?"

**🤖 AI Agent:**
> You can safely stay in the sun for 45 minutes before reaching your redness threshold.

---

**👤 You:**
> "Can I get enough Vitamin D today with a UV index of 3 and skin type IV?"

**🤖 AI Agent:**
> The synthesis capability is Optimal, with a recommended exposure of 15 minutes.


## ❓ FAQ

**Q: How does skin type affect the risk?**
The tool uses the Fitzpatrick scale to determine your skin's natural resistance to UV radiation, which directly impacts the `calculate_sunburn_risk` results.

**Q: Can I use this to plan my Vitamin D intake?**
Yes, you can use `estimate_vitamin_d_potential` to find the optimal window for Vitamin D synthesis without excessive UV damage.

**Q: Does sunscreen change the results?**
Yes, providing an SPF value to tools like `get_safe_exposure_window` will adjust the calculated safe time based on the protection provided.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/uv-exposure-risk-calculator](https://vinkius.com/en/ai-agent-connect/uv-exposure-risk-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UV Exposure Risk Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uv-exposure-risk-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UV Exposure Risk Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uv-exposure-risk-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
