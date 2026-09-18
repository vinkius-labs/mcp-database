# Sleep Apnea Risk Screener MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sleep-apnea-risk-screener)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Clinical screening tool for Obstructive Sleep Apnea risk using STOP-BANG.

## Description
This MCP server provides clinical tools to evaluate Obstructive Sleep Apnea (OSA) risk. It uses the validated STOP-BANG questionnaire alongside anthropometric data like BMI and neck circumference. Clinicians can use `calculate_osa_risk` to determine risk scores and categories, `get_risk_factor_details` to understand specific risk components, `evaluate_gender_specific_risk` for gender-nuanced interpretations, and `get_clinical_guidelines` to retrieve standardized medical recommendations.


## Available Tools (4)
- **get_clinical_guidelines**: Returns standardized clinical recommendations based on the calculated risk level
- **get_risk_factor_details**: Provides a detailed breakdown of which specific STOP-BANG criteria were met
- **calculate_osa_risk**: Performs the primary calculation of the OSA risk score and categorization based on patient inputs
- **evaluate_gender_specific_risk**: Adjusts the interpretation of the risk assessment based on gender-specific clinical nuances


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Apnea Risk Screener** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the OSA risk for a 55-year-old male with a BMI of 32, neck circumference of 45cm, who snores loudly, feels tired, and has high blood pressure."

**🤖 AI Agent:**
> The patient has a high risk score of 5, placing them in the High Risk category. Specific risk factors include snoring, tiredness, observed apnea, blood pressure, BMI, age, and neck circumference. Clinical recommendation: Urgent follow-up with a sleep specialist is required.

---

**👤 You:**
> "What are the clinical guidelines for a patient with an Intermediate OSA risk level?"

**🤖 AI Agent:**
> For an Intermediate risk level, the recommendation is to monitor symptoms closely and consider a formal sleep study if symptoms persist or worsen.

---

**👤 You:**
> "Provide descriptions for the risk factors: 'Snoring' and 'BMI'."

**🤖 AI Agent:**
> Snoring refers to loud breathing sounds during sleep that may indicate airway obstruction. BMI (Body Mass Index) is a measure of body fat based on height and weight that serves as a risk indicator for OSA.


## ❓ FAQ

**Q: What is the STOP-BANG questionnaire?**
STOP-BANG is a validated clinical screening tool used to assess the probability of Obstructive Sleep Apnea based on eight specific risk factors.

**Q: How can I get clinical recommendations?**
After calculating the risk score with `calculate_osa_risk`, you can use `get_clinical_guidelines` to receive standardized medical next steps and urgency levels.

**Q: Does gender affect the risk assessment?**
Yes, clinical presentation can vary. You can use `evaluate_gender_specific_risk` to adjust the risk interpretation based on the patient's gender.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sleep-apnea-risk-screener](https://vinkius.com/en/ai-agent-connect/sleep-apnea-risk-screener)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Apnea Risk Screener** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-apnea-risk-screener` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Apnea Risk Screener** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-apnea-risk-screener": {
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
