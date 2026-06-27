# PSS-10 Stress Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pss-10-stress-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate and analyze perceived stress levels using the PSS-10 scale.

## Description
This MCP server provides a complete implementation of the Perceived Stress Scale (PSS-10). It allows AI agents to retrieve standard assessment questions via `get_pss_questions`, validate user responses using `validate_pss_responses`, and perform detailed stress analysis with `calculate_stress_score`. The tool calculates total scores, applies necessary reverse scoring for specific items, classifies stress levels into Low, Moderate, or High, and identifies critical stress indicators.


## Available Tools (3)
- **calculate_stress_score**: Calculate the total PSS-10 stress score
- **get_pss_questions**: Retrieve the standard PSS-10 questions
- **validate_pss_responses**: Validate the provided PSS-10 responses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PSS-10 Stress Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you show me the questions for the PSS-10 assessment?"

**🤖 AI Agent:**
> Certainly! Here are the 10 items from the PSS-10 scale: item_1: In the last month, how often have you felt that you were unable to control important things in your life?...

---

**👤 You:**
> "I've completed my responses: item_1: 2, item_2: 3, item_3: 1, item_4: 4, item_5: 0, item_6: 2, item_7: 3, item_8: 1, item_9: 4, item_10: 2. What is my stress level?"

**🤖 AI Agent:**
> Based on your responses, your total PSS-10 score is 18, which indicates a Moderate level of perceived stress.

---

**👤 You:**
> "Check if these responses are valid: {'item_1': 5}"

**🤖 AI Agent:**
> The validation failed. The value for 'item_1' is out of the allowed range (0-4) and several required items are missing.


## ❓ FAQ

**Q: What is the PSS-10?**
The Perceived Stress Scale (PSS-10) is a widely used psychological instrument designed to measure the degree to which situations in one's life are appraised as stressful.

**Q: How do I use the `calculate_stress_score` tool?**
Provide a JSON object containing the 10 response items (e.g., 'item_1': 3) to the `responses` parameter. The tool will automatically handle reverse scoring and return your total score and stress level.

**Q: What are the valid response values?**
All responses must be integers between 0 and 4, where 0 means 'Never' and 4 means 'Very Often'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pss-10-stress-assessment](https://vinkius.com/mcp/pss-10-stress-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PSS-10 Stress Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pss-10-stress-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PSS-10 Stress Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pss-10-stress-assessment": {
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
