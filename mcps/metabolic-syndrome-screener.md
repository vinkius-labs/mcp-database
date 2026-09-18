# Metabolic Syndrome Screener MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/metabolic-syndrome-screener)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Clinical screening tool for metabolic syndrome risk assessment.

## Description
This MCP server provides clinical tools to evaluate metabolic health using standardized medical frameworks like NCEP ATP III and IDF. It allows AI agents to perform risk assessments by analyzing biometric data such as waist circumference, blood pressure, fasting glucose, HDL, and triglycerides. Using `screen_metabolic_status`, agents can determine if a patient meets the criteria for a metabolic syndrome diagnosis and identify specific intervention priorities.


## Available Tools (4)
- **get_criteria_thresholds**: Retrieves the specific numerical thresholds used by the different medical frameworks for a given profile
- **summarize_risk_profile**: Generates a high-level qualitative summary of the metabolic risk status
- **screen_metabolic_status**: Evaluates the user's metabolic health based on provided biometric and lab data
- **validate_biometric_range**: Verifies if the provided biometric inputs fall within physiologically plausible human ranges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Metabolic Syndrome Screener** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Screen a male patient with 105cm waist, 140/90 mmHg blood pressure, 110 mg/dL glucose, 35 mg/dL HDL, and 180 mg/dL triglycerides using NCEP ATP III."

**🤖 AI Agent:**
> The patient meets 3 criteria (waist circumference, blood pressure, and triglycerides) and is diagnosed with metabolic syndrome.

---

**👤 You:**
> "What are the NCEP ATP III thresholds for a female?"

**🤖 AI Agent:**
> For a female using NCEP ATP III, the waist circumference threshold is 88 cm, blood pressure is 90/60 mmHg, glucose is 100 mg/dL, HDL is 50 mg/dL, and triglycerides are 150 mg/dL.

---

**👤 You:**
> "Summarize the risk for a patient who has met 4 metabolic criteria."

**🤖 AI Agent:**
> The patient is in the High risk category due to meeting multiple metabolic syndrome criteria.


## ❓ FAQ

**Q: What medical frameworks are supported?**
The tool supports the NCEP ATP III and the IDF (International Diabetes Federation) frameworks for metabolic syndrome diagnosis.

**Q: How can I check the specific thresholds for a patient?**
You can use the `get_criteria_thresholds` tool to retrieve the exact numerical limits for waist circumference, blood pressure, glucose, and lipids based on the chosen framework and sex.

**Q: Can this tool validate if the input data is realistic?**
Yes, the `validate_biometric_range` tool checks if the provided biometric measurements fall within physiologically plausible human ranges.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/metabolic-syndrome-screener](https://vinkius.com/en/ai-agent-connect/metabolic-syndrome-screener)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Metabolic Syndrome Screener** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `metabolic-syndrome-screener` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Metabolic Syndrome Screener** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "metabolic-syndrome-screener": {
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
