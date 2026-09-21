# Lymphatic Drainage Pressure Guide MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lymphatic-drainage-pressure-guide)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Precision guidance for manual lymphatic drainage pressure, rhythm, and sequence.

## Description
This MCP server provides specialized guidance for manual lymphatic drainage (MLD) practitioners. It calculates optimal physical intensity and rhythmic tempo using `get_pressure_guidance`, identifies correct anatomical paths with `get_stroke_direction`, and establishes the mandatory order of operations via `get_treatment_sequence`. Practitioners can also ensure patient safety by using `validate_treatment_safety` to check if proposed pressure levels are appropriate for specific client conditions and congestion levels.


## Available Tools (4)
- **get_pressure_guidance**: Determines the specific physical intensity and rhythmic tempo required for a treatment
- **get_stroke_direction**: Identifies the correct anatomical direction for the massage strokes
- **get_treatment_sequence**: Provides the mandatory order of operations for a full-body or regional treatment
- **validate_treatment_safety**: Checks if a proposed treatment plan is safe for a specific client condition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lymphatic Drainage Pressure Guide** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What pressure and rhythm should I use for the lower leg with moderate congestion in a healthy client?"

**🤖 AI Agent:**
> For the lower leg with moderate congestion, the recommended pressure level is Medium and the rhythm is Slow.

---

**👤 You:**
> "What is the correct direction to drain the arm towards the axillary nodes?"

**🤖 AI Agent:**
> The direction is towards the axillary nodes, moving in a proximal direction to facilitate drainage.

---

**👤 You:**
> "Is it safe to use Firm pressure on a post-surgical client with mild congestion?"

**🤖 AI Agent:**
> No, the treatment is not safe. For a post-surgical client, the pressure should remain in the Light range.


## ❓ FAQ

**Q: How does the tool determine the correct pressure?**
The `get_pressure_guidance` tool calculates pressure by analyzing the anatomical area, the level of fluid congestion, and the client's specific health condition to ensure safety and effectiveness.

**Q: Can I use this to plan a full-body treatment?**
Yes, you can use `get_treatment_sequence` to receive a mandatory, ordered list of anatomical areas to treat, following the proximal-to-distal rule.

**Q: How do I ensure the treatment is safe for a sensitive client?**
Use the `validate_treatment_safety` tool. It checks if your proposed pressure level is safe given the client's condition and the current congestion level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lymphatic-drainage-pressure-guide](https://vinkius.com/en/ai-agent-connect/lymphatic-drainage-pressure-guide)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lymphatic Drainage Pressure Guide** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lymphatic-drainage-pressure-guide` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lymphatic Drainage Pressure Guide** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lymphatic-drainage-pressure-guide": {
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
