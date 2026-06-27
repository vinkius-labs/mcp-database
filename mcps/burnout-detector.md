# Burnout Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/burnout-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Assess burnout risk using the Maslach Burnout Inventory (MBI) model.

## Description
The Burnout Detector MCP server provides a specialized diagnostic tool based on the Maslach Burnout Inventory (MBI). It allows AI agents to quantify three critical dimensions of professional burnout: Emotional Exhaustion, Depersonalization, and Personal Accomplishment. Using tools like `calculate_burnout_metrics`, `evaluate_risk_level`, and `get_dimension_health_status`, users can process survey data to identify risk tiers ranging from Low to Severe. This server acts as a bridge for AI clients like Cursor, VS Code, Claude Desktop, and Windsurf to access professional well-being assessments via Vinkius Edge.


## Available Tools (3)
- **calculate_burnout_metrics**: Calculate burnout metrics from survey scores
- **get_dimension_health_status**: Get the health status of a specific burnout dimension
- **evaluate_risk_level**: Evaluate the overall burnout risk level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Burnout Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my burnout metrics with these exhaustion scores: [80, 90] and depersonalization scores: [70, 75]."

**🤖 AI Agent:**
> The calculated emotional exhaustion score is 85.0, the depersonalization score is 72.5, and your overall burnout index is being processed.

---

**👤 You:**
> "What is my risk level if my exhaustion is 90, depersonalization is 85, and accomplishment is 10?"

**🤖 AI Agent:**
> Your risk level is Severe. The high levels of exhaustion and depersonalization combined with very low accomplishment indicate extreme burnout.

---

**👤 You:**
> "Check the health status for 'Personal Accomplishment' with a score of 85."

**🤖 AI Agent:**
> The status for Personal Accomplishment is Stable, and this represents a positive trend in your professional well-being.


## ❓ FAQ

**Q: What is the Burnout Detector?**
It is a diagnostic tool based on the Maslach Burnout Inventory (MBI) that evaluates emotional exhaustion, depersonalization, and personal accomplishment.

**Q: How do I use the `calculate_burnout_metrics` tool?**
Provide arrays of numerical scores for exhaustion, depersonalization, and accomplishment. The tool will return the average score for each dimension and an overall burnout index.

**Q: What does a 'High' risk level mean?**
A High risk level indicates that visible depletion and cynicism are present, which can significantly impact work quality.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/burnout-detector](https://vinkius.com/mcp/burnout-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Burnout Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `burnout-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Burnout Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "burnout-detector": {
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
