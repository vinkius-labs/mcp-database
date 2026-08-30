# Indoor Air Quality Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/indoor-air-quality-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Evaluates chemical laboratory safety through IAQ indexing and ventilation analysis.

## Description
This MCP server provides specialized tools for chemical laboratory safety management. It allows AI agents to calculate the `calculate_iaq_index` to determine overall air quality health, use `get_contaminant_ratios` to identify specific chemical risks, and run `evaluate_ventilation_adequacy` to ensure airflow meets safety standards. For a complete overview, `analyze_lab_safety_profile` aggregates all data into a single safety report.


## Available Tools (4)
- **analyze_lab_safety_profile**: To provide a comprehensive summary of the lab's chemical and ventilation status
- **calculate_iaq_index**: To determine the overall air quality health score for a laboratory
- **evaluate_ventilation_adequacy**: To determine if the current airflow is sufficient to maintain safety given the laboratory's usage
- **get_contaminant_ratios**: To identify how close each individual chemical is to its safe breathing limit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Indoor Air Quality Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the IAQ index for a lab with Benzene at 0.5 ppm and Toluene at 2.0 ppm, where limits are Benzene 0.1 ppm and Toluene 5.0 ppm."

**🤖 AI Agent:**
> The IAQ index is 5.0, with Benzene identified as the primary contaminant causing a Critical status.

---

**👤 You:**
> "Is the ventilation adequate for a 100m3 room with a 50m3/h ventilation rate, 2 people, and a target of 6 air changes per hour?"

**🤖 AI Agent:**
> No, the ventilation is not adequate. The current adequacy score is 8.33%, and a required rate of 600m3/h is needed to meet the target.

---

**👤 You:**
> "Provide a safety profile for a lab with CO2 at 400ppm (limit 1000), Ammonia at 15ppm (limit 25), and ventilation rate of 200m3/h in a 50m3 room with 1 person and target 5 ACH."

**🤖 AI Agent:**
> The lab has a Low Risk profile. The IAQ index is 0.4, ventilation is adequate, and all contaminant levels are well within safe limits.


## ❓ FAQ

**Q: What can this tool calculate?**
It calculates the IAQ index, individual contaminant ratios, ventilation adequacy, and a full laboratory safety profile.

**Q: How is ventilation adequacy determined?**
It compares the actual air changes per hour against the target air changes required for the specific laboratory classification.

**Q: Can I assess multiple contaminants at once?**
Yes, the tools are designed to handle arrays of contaminant measurements and their corresponding exposure limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/indoor-air-quality-assessment](https://vinkius.com/ai-agent-connect/indoor-air-quality-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Indoor Air Quality Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `indoor-air-quality-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Indoor Air Quality Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "indoor-air-quality-assessment": {
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
