# Shockwave Therapy Protocol Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shockwave-therapy-protocol-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Generates precise clinical shockwave therapy parameters based on patient condition and chronicity.

## Description
This MCP server provides clinical decision support for Extracorporeal Shockwave Therapy (ESWT). It allows AI agents to calculate specific therapeutic settings including energy flux density, impulse count, and frequency. Clinicians can use `get_protocol_parameters` to determine session settings, `validate_area_safety` to ensure anatomical appropriateness, `get_chronicity_guidelines` to understand biological healing phases, and `get_treatment_frequency_schedule` to plan the full course of treatment.


## Available Tools (4)
- **get_chronicity_guidelines**: Retrieves standard biological expectations for different disease durations
- **get_protocol_parameters**: Calculates specific therapeutic settings for a single treatment session
- **get_treatment_frequency_schedule**: Determines the full course of treatment
- **validate_area_safety**: Checks if the requested treatment area is appropriate for the specific condition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shockwave Therapy Protocol Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the shockwave parameters for chronic Plantar Fasciitis on the foot with medium patient tolerance?"

**🤖 AI Agent:**
> For chronic Plantar Fasciitis on the foot with medium tolerance, the target energy flux density is 0.25 mJ/mm², with 2500 impulses at a frequency of 15 Hz. The recommended treatment interval is once weekly.

---

**👤 You:**
> "Is it safe to treat Achilles Tendinopathy in the ankle area?"

**🤖 AI Agent:**
> Yes, treatment for Achilles Tendinopathy in the ankle area is considered safe according to the clinical guidelines.

---

**👤 You:**
> "What is the biological phase for an acute condition?"

**🤖 AI Agent:**
> An acute condition is typically in the Inflammatory biological phase, requiring a low-energy stimulation strategy.


## ❓ FAQ

**Q: How do I determine the energy settings for a patient?**
You can use the `get_protocol_parameters` tool, providing the condition, chronicity, treatment area, and patient tolerance to receive specific energy flux density and impulse counts.

**Q: Can I check if a treatment area is safe for a specific condition?**
Yes, the `validate_area_safety` tool is designed to verify if a requested treatment area is appropriate for the clinical diagnosis.

**Q: How many sessions will a patient typically need?**
The `get_treatment_frequency_schedule` tool provides the recommended total number of sessions and the session cadence based on the condition and chronicity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shockwave-therapy-protocol-planner](https://vinkius.com/en/ai-agent-connect/shockwave-therapy-protocol-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shockwave Therapy Protocol Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shockwave-therapy-protocol-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shockwave Therapy Protocol Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shockwave-therapy-protocol-planner": {
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
