# Hypoglycemia Recovery Protocol MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hypoglycemia-recovery-protocol)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Deterministic 'Rule of 15' calculator for immediate hypoglycemia treatment.

## Description
This MCP server provides clinical decision support for managing hypoglycemic episodes using the standard 'Rule of 15' protocol. It calculates the exact amount of carbohydrates needed based on the selected source to ensure a consistent 15g dose. Users can determine if immediate treatment is required, predict blood glucose rise using an Insulin Sensitivity Factor (ISF), and identify if a second round of treatment is necessary. Use `calculate_hypoglycemia_intervention` to get a full treatment plan, `validate_carb_source_availability` to check supported sources, or `get_carb_density_conversion` for specific carbohydrate density data.


## Available Tools (3)
- **validate_carb_source_availability**: Verify if a carb source is supported
- **calculate_hypoglycemia_intervention**: 
- **get_carb_density_conversion**: Get conversion constants for carb sources


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hypoglycemia Recovery Protocol** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My blood glucose is 65 mg/dL. I have juice available. My ISF is 50. What should I do?"

**🤖 AI Agent:**
> Treatment is required. You should consume 125ml of juice. This is expected to raise your blood glucose by 750 mg/dL, resulting in a projected blood glucose of 815 mg/dL.

---

**👤 You:**
> "I have 55 mg/dL blood glucose. I'm using glucose tabs. My ISF is 40. What is the plan?"

**🤖 AI Agent:**
> Treatment is required. Consume 4 tabs of glucose. This will result in an expected rise of 600 mg/dL, with a projected blood glucose of 655 mg/dL.

---

**👤 You:**
> "Is honey a valid source for the hypoglycemia protocol?"

**🤖 AI Agent:**
> Yes, honey is a supported carbohydrate source for this protocol.


## ❓ FAQ

**Q: What is the Rule of 15?**
The Rule of 15 is a standard medical guideline where an individual consumes 15 grams of fast-acting carbohydrates, waits 15 minutes, and then re-tests their blood glucose levels.

**Q: How do I know if I need treatment?**
You can use `calculate_hypoglycemia_intervention` to check if your current blood glucose level requires immediate corrective action.

**Q: Which carbohydrate sources are supported?**
The protocol supports glucose tablets, juice, regular soda, and honey. You can verify any source using `validate_carb_source_availability`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hypoglycemia-recovery-protocol](https://vinkius.com/ai-agent-connect/hypoglycemia-recovery-protocol)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hypoglycemia Recovery Protocol** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hypoglycemia-recovery-protocol` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hypoglycemia Recovery Protocol** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hypoglycemia-recovery-protocol": {
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
