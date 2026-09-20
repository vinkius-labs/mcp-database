# Restless Legs Severity Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/restless-legs-severity-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculates clinical severity scores for Restless Legs Syndrome (RLS) using the IRLSSG scale.

## Description
This MCP server provides clinical tools to quantify the severity of Restless Legs Syndrome (RLS). It uses the International Restless Legs Syndrome Study Group (IRLSSG) methodology to process symptom intensity, frequency, and sleep impact. Users can use `calculate_rls_score` to determine a severity category, `get_ferritin_recommendation` to identify the need for iron testing, and `get_treatment_considerations` to outline clinical management themes. It also includes `validate_irlssg_inputs` to ensure all questionnaire data falls within valid clinical ranges.


## Available Tools (4)
- **calculate_rls_score**: Calculates the primary clinical severity score and determines the diagnostic category
- **get_ferritin_recommendation**: Determines if blood testing for iron (ferritin) is clinically indicated
- **get_treatment_considerations**: Provides high-level clinical themes and considerations for management
- **validate_irlssg_inputs**: Ensures that individual questionnaire components are within valid bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Restless Legs Severity Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the RLS severity for a patient with an intensity of 3, frequency of 2, and sleep impact of 3."

**🤖 AI Agent:**
> The calculated total score is 8, which falls into the Moderate severity category.

---

**👤 You:**
> "Should a patient with a severity score of 9 and daily symptoms undergo ferritin testing?"

**🤖 AI Agent:**
> Yes, ferritin testing is recommended with immediate urgency due to the high severity score and daily symptom presence.

---

**👤 You:**
> "What are the treatment considerations for a patient in the Severe category?"

**🤖 AI Agent:**
> For the Severe category, clinical themes include pharmacological evaluation and intensive monitoring.


## ❓ FAQ

**Q: What scale does this server use?**
The server utilizes the International Restless Legs Syndrome Study Group (IRLSSG) scale to ensure standardized clinical scoring.

**Q: Can I get iron deficiency recommendations?**
Yes, by using the `get_ferritin_recommendation` tool, the server provides guidance on whether ferritin testing is indicated based on the severity score and symptom frequency.

**Q: Is this tool suitable for clinical decision support?**
This server is designed to assist in quantifying symptoms and providing clinical themes, but it should be used as a support tool alongside professional medical judgment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/restless-legs-severity-scorer](https://vinkius.com/en/ai-agent-connect/restless-legs-severity-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Restless Legs Severity Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `restless-legs-severity-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Restless Legs Severity Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "restless-legs-severity-scorer": {
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
