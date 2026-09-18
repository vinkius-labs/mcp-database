# Blood Pressure Category Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/blood-pressure-category-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Categorizes blood pressure readings and assesses cardiovascular risk using international guidelines.

## Description
This MCP server provides clinical decision support for blood pressure management. It uses `assess_blood_pressure` to classify readings into categories like Normal, Elevated, or Hypertensive Crisis based on systolic and diastolic values. It also provides `get_lifestyle_guidelines` for tailored dietary and activity advice, `calculate_monitoring_schedule` to determine checkup frequency, and `compare_guideline_standards` to evaluate readings against both ACC/AHA and ESC/ESH international standards.


## Available Tools (4)
- **assess_blood_pressure**: Performs the primary clinical classification of a single blood pressure reading
- **calculate_monitoring_schedule**: Determines how frequently a patient should monitor their blood pressure
- **compare_guideline_standards**: Compares a patient's current reading against different international standards
- **get_lifestyle_guidelines**: Retrieves specific, evidence-based lifestyle modifications tailored to a patient's risk profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blood Pressure Category Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Assess a blood pressure reading of 145/95 mmHg for a 55-year-old with diabetes."

**🤖 AI Agent:**
> The blood pressure is categorized as Stage 2 Hypertension. Given the presence of diabetes, the cardiovascular risk stage is high. It is recommended to monitor blood pressure daily and focus on sodium reduction in your diet.

---

**👤 You:**
> "What are the lifestyle recommendations for a low risk profile?"

**🤖 AI Agent:**
> For a low risk profile, it is recommended to maintain a balanced diet, engage in regular moderate physical activity, and manage weight through healthy eating habits.

---

**👤 You:**
> "How often should someone with Stage 1 hypertension monitor their blood pressure?"

**🤖 AI Agent:**
> For Stage 1 hypertension, monitoring is typically recommended weekly or monthly depending on the specific risk stage and presence of other conditions.


## ❓ FAQ

**Q: Which clinical guidelines are used for assessment?**
The tool utilizes both ACC/AHA and ESC/ESH international guidelines to ensure standardized classification and risk assessment.

**Q: Can I get lifestyle recommendations based on my risk level?**
Yes, you can use `get_lifestyle_guidelines` to receive specific dietary and physical activity recommendations tailored to your risk profile and existing medical conditions.

**Q: How does the tool handle white coat hypertension?**
The `assess_blood_pressure` tool allows you to specify if a reading is identified as white coat hypertension, which may result in a lower risk tier classification per clinical guidance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/blood-pressure-category-assessment](https://vinkius.com/en/ai-agent-connect/blood-pressure-category-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blood Pressure Category Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blood-pressure-category-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blood Pressure Category Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blood-pressure-category-assessment": {
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
