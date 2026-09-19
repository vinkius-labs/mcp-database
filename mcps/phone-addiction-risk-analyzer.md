# Phone Addiction Risk Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/phone-addiction-risk-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantifies smartphone dependency risk using validated behavioral metrics.

## Description
This MCP server provides tools to assess smartphone addiction risk by analyzing usage patterns. It uses `calculate_risk_score` to evaluate daily pickups, screen time, social media intensity, and psychological indicators like phantom vibration syndrome. Users can also use `get_category_details` to understand risk levels or `get_intervention_guide` to receive actionable behavioral advice to reduce digital dependency.


## Available Tools (4)
- **get_category_details**: Provides descriptive definitions and threshold information for the addiction categories
- **get_intervention_guide**: Retrieves a list of specific behavioral interventions for a given risk level
- **calculate_risk_score**: Generates a comprehensive addiction risk score and classification for a user
- **validate_usage_metrics**: Checks if the provided usage data is physically and logically possible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Phone Addiction Risk Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my phone addiction risk. I have 100 pickups, 300 minutes of screen time, 150 minutes on social media, a responsiveness of 8, and I do experience phantom vibrations."

**🤖 AI Agent:**
> Your addiction risk score is 75, which falls into the High Risk category. It is recommended that you set strict app limits and practice digital detox periods.

---

**👤 You:**
> "What are the details for the Moderate Risk category?"

**🤖 AI Agent:**
> The Moderate Risk category represents noticeable interference with focus or sleep, with a score range of 30 to 59.

---

**👤 You:**
> "Give me some interventions for a Low Risk level."

**🤖 AI Agent:**
> For Low Risk, try hygiene strategies such as disabling non-essential notifications and keeping your phone away from your bed at night.


## ❓ FAQ

**Q: How is the addiction risk calculated?**
The score is calculated using `calculate_risk_score`, which weights daily pickups, screen time, social media usage, notification responsiveness, and the presence of phantom vibration syndrome.

**Q: Can I get advice on how to reduce my phone usage?**
Yes, you can use `get_intervention_guide` to receive specific behavioral recommendations tailored to your calculated risk category.

**Q: What if my usage data is invalid?**
You can use `validate_usage_metrics` to ensure your daily pickups and screen time are logically consistent before running a full assessment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/phone-addiction-risk-analyzer](https://vinkius.com/en/ai-agent-connect/phone-addiction-risk-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Phone Addiction Risk Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `phone-addiction-risk-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Phone Addiction Risk Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "phone-addiction-risk-analyzer": {
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
