# MEWS Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mews-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Quantify patient physiological deterioration using the Modified Early Warning Score (MEWS) system.

## Description
The MEWS Calculator is a clinical assessment tool designed to identify patients at risk of clinical deterioration. By analyzing vital signs such as respiratory rate, SpO2, heart rate, systolic blood pressure, body temperature, and consciousness level (AVPU), it calculates a cumulative score. Use the `calculate_mews_score` tool to compute the numerical score, `get_clinical_classification` to determine risk levels, and `check_activation_threshold` to see if a Rapid Response Team activation is necessary.


## Available Tools (3)
- **check_activation_threshold**: Checks if a MEWS score requires activation of the Rapid Response Team
- **calculate_mews_score**: Calculates the cumulative MEWS score based on vital signs
- **get_clinical_classification**: Determines the clinical risk category based on a MEWS score


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MEWS Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the MEWS score for a patient with RR 24, SpO2 92%, HR 110, SBP 95, Temp 38.5, and level V."

**🤖 AI Agent:**
> The calculated MEWS score is 5.

---

**👤 You:**
> "What is the clinical risk for a patient with a MEWS score of 2?"

**🤖 AI Agent:**
> A MEWS score of 2 indicates a Low Risk status.

---

**👤 You:**
> "Does a MEWS score of 6 require RRT activation?"

**🤖 AI Agent:**
> Yes, a score of 6 meets the threshold. Action Required: Activate Rapid Response.


## ❓ FAQ

**Q: What is the MEWS score?**
The Modified Early Warning Score (MEWS) is a numerical value calculated from vital signs to assess the risk of clinical deterioration in patients.

**Q: How do I use the `calculate_mews_score` tool?**
Provide the patient's respiratory rate, SpO2, heart rate, systolic blood pressure, body temperature, and consciousness level (AVPU) to receive the calculated score.

**Q: When should a Rapid Response Team be activated?**
You can use the `check_activation_threshold` tool to determine if the current MEWS score meets the threshold for emergency activation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mews-calculator](https://vinkius.com/mcp/mews-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MEWS Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mews-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MEWS Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mews-calculator": {
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
