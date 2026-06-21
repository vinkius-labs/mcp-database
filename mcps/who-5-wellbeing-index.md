# WHO-5 Wellbeing Index MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/who-5-wellbeing-index)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate the WHO-5 Well-Being Index score and identify potential wellbeing risks.

## Description
This MCP server provides specialized tools to quantify psychological well-being using the World Health Organization's WHO-5 scale. Use `calculate_wellbeing_assessment` to input five responses (0-5) and receive a normalized score from 0 to 100, along with a wellbeing classification and risk assessment. You can also use `fetch_scale_instructions` to understand the numeric mapping for each response or `validate_assessment_range` to verify if a specific score falls within the standard valid bounds.


## Available Tools
- **validate_assessment_range**: Verifies if a score is within the 0-100 range
- **calculate_wellbeing_assessment**: Calculates the WHO-5 Well-Being Index score
- **fetch_scale_instructions**: Provides context for the WHO-5 scale


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WHO-5 Wellbeing Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my wellbeing score with these responses: 5, 4, 5, 4, 5."

**🤖 AI Agent:**
> The `calculate_wellbeing_assessment` tool would return a score of 90, indicating Normal Wellbeing with no high-risk indicators detected.

---

**👤 You:**
> "What does the scale mapping look like?"

**🤖 AI Agent:**
> By using `fetch_scale_instructions`, you can see that 0 represents 'Never' and 5 represents 'All the time'.

---

**👤 You:**
> "Is a score of 45 valid?"

**🤖 AI Agent:**
> The `validate_assessment_range` tool would confirm that 45 is within the valid range (0-100), though it indicates a low wellbeing state.


## ❓ FAQ

**Q: What is the WHO-5 Well-Being Index?**
The WHO-5 is a screening tool used to assess subjective psychological well-being based on how an individual has felt over the last two weeks.

**Q: How do I interpret the score?**
The score is normalized to a 0-100 scale. A score below 50 is considered a significant indicator of potential low well-being.

**Q: What inputs are required for the assessment?**
You need to provide five numeric responses, each ranging from 0 (never) to 5 (all the time), corresponding to the five questions in the scale.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/who-5-wellbeing-index](https://vinkius.com/mcp/who-5-wellbeing-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WHO-5 Wellbeing Index** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `who-5-wellbeing-index` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WHO-5 Wellbeing Index** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "who-5-wellbeing-index": {
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
