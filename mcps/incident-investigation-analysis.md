# Incident Investigation Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/incident-investigation-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analysis](../categories/analysis.md)

Analyze incident data using root cause methodologies like 5-Why and Fishbone.

## Description
This MCP server provides a structured framework for investigating incidents. It allows AI agents to organize raw incident narratives using `analyze_incident_structure`, perform deep dives with `perform_root_cause_analysis` (supporting 5-Why, Fishbone, and TapRooT), identify organizational flaws via `evaluate_management_factors`, and build actionable roadmaps with `generate_mitigation_plan`.


## Available Tools (4)
- **evaluate_management_factors**: Investigates how organizational systems allowed the incident to occur
- **generate_mitigation_plan**: Produces a roadmap of actions to prevent future occurrences
- **perform_root_cause_analysis**: Applies specific methodologies to determine the underlying causes of the incident
- **analyze_incident_structure**: Organizes raw incident data into a structured format ready for deep analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Incident Investigation Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this incident: A technician slipped on an oil leak in the main hangar."

**🤖 AI Agent:**
> The incident summary indicates a slip hazard due to an oil leak in the main hangar, with a Medium severity level.

---

**👤 You:**
> "Perform a 5-Why analysis for incident ID INC-101 with causal factors: 'Broken valve' and 'High pressure'."

**🤖 AI Agent:**
> The root cause is identified as a failure in the scheduled preventative maintenance program for high-pressure valves.

---

**👤 You:**
> "Generate a mitigation plan for the root cause: 'Lack of operator training'."

**🤖 AI Agent:**
> Corrective Action: Implement a mandatory quarterly training certification for all operators. Target Timeline: Within 30 days.


## ❓ FAQ

**Q: What methodologies can I use for analysis?**
You can use 5-Why, Fishbone, or TapRooT through the `perform_root_cause_analysis` tool.

**Q: How does the tool handle organizational issues?**
The `evaluate_management_factors` tool maps root causes to systemic weaknesses in policy, training, or culture.

**Q: Can I generate a plan to prevent recurrence?**
Yes, the `generate_mitigation_plan` tool produces specific corrective actions and strategic recommendations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/incident-investigation-analysis](https://vinkius.com/en/ai-agent-connect/incident-investigation-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Incident Investigation Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `incident-investigation-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Incident Investigation Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "incident-investigation-analysis": {
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
