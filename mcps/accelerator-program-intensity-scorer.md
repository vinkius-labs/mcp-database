# Accelerator Program Intensity Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-program-intensity-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Quantify operational pressure and burnout risk in startup accelerator programs.

## Description
This MCP server provides specialized tools to measure the cognitive and temporal load of startup accelerators. By analyzing weekly hours, curriculum density, and milestone frequency, it calculates a precise intensity score. It helps program designers identify burnout risks for different founder experience levels and ensures that program pressure is appropriately aligned with a startup's current lifecycle stage.


## Available Tools (3)
- **analyze_stage_alignment**: Determines if the proposed program intensity is appropriate for a startup's current stage of development
- **calculate_intensity_metrics**: Provides a comprehensive snapshot of the program's impact including the intensity score, risk, and ideal targets
- **get_burnout_thresholds**: Retrieves the specific intensity score limits that trigger different risk levels for different founder profiles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Program Intensity Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the intensity metrics for a program requiring 40 hours a week, 0.8 curriculum density, 4 milestones per month, 0.5 support intensity, for an expert founder in the seed stage."

**🤖 AI Agent:**
> The program has an intensity score of 7.5, a low burnout risk for an expert founder, and is well-aligned for the seed stage.

---

**👤 You:**
> "What are the burnout thresholds for a novice founder?"

**🤖 AI Agent:**
> For a novice founder, the low risk limit is 3.0, the medium risk limit is 5.5, and the high risk limit is 8.0.

---

**👤 You:**
> "Is an intensity score of 9 appropriate for an ideation stage startup?"

**🤖 AI Agent:**
> No, an intensity score of 9 is not aligned with the ideation stage; it is too high and may lead to immediate burnout.


## ❓ FAQ

**Q: How is the intensity score calculated?**
The score is derived using `calculate_intensity_metrics`, which combines workload (hours and density) with pressure (milestones) and adjusts for support intensity and stage alignment.

**Q: Can I check if a program is too intense for a specific founder?**
Yes, you can use `get_burnout_thresholds` to retrieve specific intensity limits for novice, intermediate, or expert founder profiles.

**Q: How do I know if the program matches the startup's stage?**
You can use `analyze_stage_alignment` to compare a target intensity score against the expected requirements for stages like ideation, seed, or growth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-program-intensity-scorer](https://vinkius.com/ai-agent-connect/accelerator-program-intensity-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Program Intensity Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-program-intensity-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Program Intensity Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-program-intensity-scorer": {
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
