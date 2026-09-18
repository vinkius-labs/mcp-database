# Purpose in Life Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/purpose-in-life-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [wellness](../categories/wellness.md)

Assess your sense of purpose, clarity, and engagement through psychometric analysis.

## Description
This MCP server provides a suite of psychological assessment tools to help you understand your sense of meaning. By analyzing your responses, you can use `get_purpose_score` to calculate your overall purpose metric, `get_clarity_profile` to measure life directionality, `get_engagement_metrics` to evaluate how actively you live your values, and `get_purpose_activities` to receive tailored recommendations for personal growth.


## Available Tools (4)
- **get_clarity_profile**: Analyzes the degree of ambiguity versus direction in the user's life
- **get_engagement_metrics**: Evaluates how actively a person is living out their perceived meaning
- **get_purpose_activities**: Recommends specific types of activities to increase or sustain purpose
- **get_purpose_score**: Calculates the primary purpose metric based on raw assessment responses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Purpose in Life Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my purpose score with responses [5, 4, 5, 3] and a goal pursuit intensity of 4."

**🤖 AI Agent:**
> Your calculated purpose score is 4.2, with a clarity score of 3.8 and an engagement score of 4.0.

---

**👤 You:**
> "What is my clarity profile based on these responses: [3, 2, 3, 4]?"

**🤖 AI Agent:**
> Your clarity level is Moderate, with an ambiguity level of 2.5 and a primary direction of Exploration.

---

**👤 You:**
> "Suggest some activities for someone with a purpose score of 8 and a clarity score of 7."

**🤖 AI Agent:**
> Based on your high scores, we recommend focusing on Implementation and Community Contribution through activities like Mentorship or Volunteering.


## ❓ FAQ

**Q: How is the purpose score calculated?**
The score is a weighted combination of your assessment responses and your reported goal pursuit intensity.

**Q: Can I get recommendations for activities?**
Yes, you can use the `get_purpose_activities` tool to receive specific activity categories based on your purpose and clarity scores.

**Q: What does clarity of purpose mean?**
Clarity measures how well you understand your long-term objectives and the values driving your life direction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/purpose-in-life-assessment](https://vinkius.com/en/ai-agent-connect/purpose-in-life-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Purpose in Life Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `purpose-in-life-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Purpose in Life Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "purpose-in-life-assessment": {
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
