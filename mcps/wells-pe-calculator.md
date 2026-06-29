# Wells PE Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wells-pe-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate Wells Score for Pulmonary Embolism and determine diagnostic pathways.

## Description
This MCP server provides clinical decision support for assessing pulmonary embolism risk. Using the `wellsScoreTool`, clinicians can calculate the Wells Score based on seven clinical criteria to determine pre-test probability. Additionally, the `percRuleTool` evaluates if a patient meets the Pulmonary Embolism Rule-out Criteria (PERC), and the `diagnosticPathwayTool` recommends the next diagnostic step, such as CTPA or D-dimer testing, following ESC/ATS guidelines.


## Available Tools (3)
- **determine_diagnostic_pathway**: Determine the diagnostic pathway for PE
- **evaluate_perc_prob**: Evaluate the PERC rule for PE
- **calculate_wells_score**: Calculate the Wells Score for Pulmonary Embolism


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wells PE Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Wells Score for a patient with tachycardia and recent surgery."

**🤖 AI Agent:**
> The calculated Wells Score is 3, placing the patient in the Low probability category.

---

**👤 You:**
> "What should I do if a patient has a high Wells score?"

**🤖 AI Agent:**
> For patients in the High probability group, the recommended action is to perform CT Pulmonary Angiography (CTPA).

---

**👤 You:**
> "Check if a 25-year-old patient with no symptoms passes the PERC rule."

**🤖 AI Agent:**
> The patient meets all criteria and is considered PERC negative, meaning no further testing is required.


## ❓ FAQ

**Q: What clinical criteria are used in the Wells Score?**
The tool assesses seven criteria including DVT signs, PE as most likely diagnosis, tachycardia, recent immobilization or surgery, previous VTE history, hemoptysis, and active malignancy.

**Q: How does the tool recommend next steps?**
By using `diagnosticPathwayTool`, it follows ESC/ATS guidelines to suggest actions like CTPA, D-dimer testing, or discharge based on risk levels.

**Q: Does this tool support the PERC rule?**
Yes, the `percRuleTool` allows clinicians to evaluate if a patient can be safely ruled out for PE using clinical observation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wells-pe-calculator](https://vinkius.com/mcp/wells-pe-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wells PE Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wells-pe-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wells PE Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wells-pe-calculator": {
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
