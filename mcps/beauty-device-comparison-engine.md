# Beauty Device Comparison Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/beauty-device-comparison-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [beauty-tech](../categories/beauty-tech.md)

Compare at-home beauty tech devices based on skin type, budget, and clinical efficacy.

## Description
The Beauty Device Comparison Engine connects AI agents to a specialized database of 80+ at-home beauty technologies. Using tools like `filter_devices`, `get_treatment_implications`, and `get_efficacy_projections`, users can evaluate devices such as LED masks, microcurrent, and RF technology. The engine matches user physiological profiles (Fitzpatrick skin scale) with clinical data to project long-term costs, time investment, and expected timelines for visible results.


## Available Tools (4)
- **compare_devices**: Compare multiple beauty devices
- **get_efficacy_projections**: Get efficacy projections for a specific device
- **filter_devices**: Filter beauty devices by skin type and concern
- **get_treatment_implications**: Get treatment implications for a specific device


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beauty Device Comparison Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me an affordable LED mask for Type IV skin that targets acne."

**🤖 AI Agent:**
> I found the Lumina-LED Pro, which is compatible with Type IV skin and specifically targets acne. It fits within your budget constraints.

---

**👤 You:**
> "What is the yearly cost and time commitment for the RF-Tighten device?"

**🤖 AI Agent:**
> The RF-Tighten device has a total yearly cost of $450 and requires a weekly time investment of 30 minutes.

---

**👤 You:**
> "Compare the efficacy timelines for device_id_123 and device_id_456."

**🤖 AI Agent:**
> device_id_123 shows visible results in 4 weeks with high confidence, while device_id_456 requires approximately 12 weeks.


## ❓ FAQ

**Q: How does the engine determine device safety?**
The engine uses the `filter_devices` tool to match your Fitzpatrick skin type with the device's clinical safety profile, ensuring technologies like lasers are only recommended for appropriate skin tones.

**Q: Can I compare multiple devices at once?**
Yes, you can use the `compare_devices` tool by providing a list of device IDs to generate a side-by-side comparison matrix.

**Q: Does the engine include long-term costs?**
Yes, by using `get_treatment_implications`, you can see the total yearly cost including device purchase and session frequency expenses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/beauty-device-comparison-engine](https://vinkius.com/mcp/beauty-device-comparison-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beauty Device Comparison Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beauty-device-comparison-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beauty Device Comparison Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beauty-device-comparison-engine": {
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
