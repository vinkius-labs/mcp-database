# Nutritional Risk Screening (NRS-2002) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nutritional-risk-screening-nrs-2002)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Assess nutritional risk in hospitalized patients using the NRS-2002 protocol and ESPEN guidelines.

## Description
This MCP server implements the validated NRS-2002 (Nutritional Risk Screening 2002) protocol to identify malnutrition risk in hospitalized patients. By evaluating Body Mass Index (BMI), recent unintended weight loss, food intake reduction, and disease severity impact, it provides a clinical score and actionable nutritional support recommendations following ESPEN guidelines. Use `perform_full_nrs_screening` for a complete assessment or individual tools like `evaluate_nutritional_status` and `evaluate_disease_impact` for specific component scoring.


## Available Tools (3)
- **evaluate_disease_impact**: Calculate the disease impact score (S component) of NRS-20 $	ext{02}$
- **evaluate_nutritional_status**: Calculate the nutritional status score (N component) of NRS-20 $	ext{02}$
- **perform_full_nrs_screening**: Perform a complete NRS-2002 nutritional risk screening


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nutritional Risk Screening (NRS-2002)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Perform a full NRS-2002 screening for a patient with BMI 18.5, 5% weight loss, reduced food intake, and moderate disease severity."

**🤖 AI Agent:**
> The complete nutritional risk screening results in a total score of 3, classifying the patient as High Risk. Nutritional Intervention Required is recommended.

---

**👤 You:**
> "Check the nutritional status score for a patient with BMI 24, no weight loss, and normal food intake."

**🤖 AI Agent:**
> The nutritional status score (N component) is 0.

---

**👤 You:**
> "What is the impact of high disease severity on the NRS-2002 score?"

**🤖 AI Agent:**
> A high severity level adds 2 points to the total screening score, increasing the overall nutritional risk assessment.


## ❓ FAQ

**Q: What is the purpose of this tool?**
It identifies patients at risk of malnutrition during hospital stays by calculating a score based on nutritional status and disease severity.

**Q: How is the risk determined?**
The tool aggregates points from BMI, weight loss, food intake, and metabolic stress. A total score of 3 or higher indicates nutritional risk.

**Q: Does it follow any specific guidelines?**
Yes, the clinical recommendations provided are based on the European Society for Clinical Nutrition and Metabolism (ESPEN) guidelines.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nutritional-risk-screening-nrs-2002](https://vinkius.com/mcp/nutritional-risk-screening-nrs-2002)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nutritional Risk Screening (NRS-2002)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nutritional-risk-screening-nrs-2002` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nutritional Risk Screening (NRS-2002)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nutritional-risk-screening-nrs-2002": {
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
