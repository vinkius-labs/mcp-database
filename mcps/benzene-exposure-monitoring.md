# Benzene Exposure Monitoring MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/benzene-exposure-monitoring)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industrial-hygiene](../categories/industrial-hygiene.md)

Design and manage occupational health programs for benzene exposure monitoring.

## Description
This MCP server provides specialized tools for managing benzene exposure in industrial environments. It allows users to `plan_sampling_strategy` based on specific work activities and risk profiles, `calculate_exposure_thresholds` for different regulatory regions like the USA or Europe, and `evaluate_compliance_risk` to detect TWA or STEL violations. Additionally, it can `generate_medical_surveillance_plan` to ensure worker health is monitored according to exposure levels.


## Available Tools (4)
- **calculate_exposure_thresholds**: Calculates the specific TWA, STEL, and Action Levels for a given regulatory environment
- **evaluate_compliance_risk**: Assesses the risk of exceeding limits based on current monitoring data
- **generate_medical_surveillance_plan**: Creates a health monitoring schedule based on exposure levels and duration
- **plan_sampling_strategy**: Determines the appropriate method and frequency for air sampling based on work context


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Benzene Exposure Monitoring** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me plan a sampling strategy for a high-risk facility with benzene in fuel refining and tank cleaning activities."

**🤖 AI Agent:**
> The recommended sampling methodology for high-risk fuel refining and tank cleaning is continuous air monitoring with a frequency of daily checks for workers in direct contact with sources.

---

**👤 You:**
> "What are the exposure thresholds for benzene in the USA with a base TWA of 1.0 ppm?"

**🤖 AI Agent:**
> For a base TWA of 1.0 ppm in the USA, the STEL limit is 5.0 ppm and the action level is 0.5 ppm.

---

**👤 You:**
> "A worker has been exposed to moderate levels of benzene for 5 years. What is the medical surveillance plan?"

**🤖 AI Agent:**
> The medical surveillance plan requires annual biological monitoring of specific biomarkers with a review scheduled for next year.


## ❓ FAQ

**Q: How do I determine how often to sample for benzene?**
You can use the `plan_sampling_strategy` tool. By providing the benzene sources, work activities, and the risk profile, the tool will return a recommended frequency and methodology.

**Q: Can this tool help with regulatory compliance in the USA?**
Yes. Use `calculate_exposure_thresholds` with the USA regulatory region to find the specific TWA and STEL limits required for compliance.

**Q: What happens if a benzene concentration exceeds the limit?**
You can use `evaluate_compliance_risk` to check if a measured concentration is a violation. If the status is 'action_required' or 'exceeded', immediate intervention is necessary.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/benzene-exposure-monitoring](https://vinkius.com/en/ai-agent-connect/benzene-exposure-monitoring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Benzene Exposure Monitoring** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `benzene-exposure-monitoring` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Benzene Exposure Monitoring** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "benzene-exposure-monitoring": {
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
