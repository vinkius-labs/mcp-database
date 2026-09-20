# Insomnia Severity Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/insomnia-severity-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Clinical-grade monitoring for insomnia severity, trends, and intervention efficacy.

## Description
This MCP server provides clinical-grade tools to monitor insomnia progression. It allows AI agents to determine severity levels using `calculate_current_severity`, evaluate progression via `analyze_severity_trend`, measure the success of treatments with `evaluate_intervention_efficacy`, and identify when medical consultation is required through `check_referral_necessity`.


## Available Tools (4)
- **evaluate_intervention_efficacy**: Measures how much a specific intervention has reduced insomnia symptoms
- **analyze_severity_trend**: Evaluates the direction and velocity of insomnia progression over time
- **calculate_current_severity**: Determines the current clinical severity level based on the most recent assessment
- **check_referral_necessity**: Identifies if the patient's symptoms require professional medical consultation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Insomnia Severity Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current insomnia severity if my ISI score is 22?"

**🤖 AI Agent:**
> Your current insomnia severity is severe.

---

**👤 You:**
> "Is my insomnia getting better? My previous scores were 20, 18, and 15."

**🤖 AI Agent:**
> Your insomnia severity is improving.

---

**👤 You:**
> "I had an ISI score of 20 before my new sleep routine and now it is 12. How effective was it?"

**🤖 AI Agent:**
> The intervention was highly effective, resulting in a 40% reduction in severity.


## ❓ FAQ

**Q: What is the Insomnia Severity Index (ISI)?**
The ISI is a standardized metric used to assess the severity of insomnia symptoms.

**Q: How can I check if my symptoms require a doctor?**
You can use the `check_referral_necessity` tool to determine if your current severity and functional impact warrant a medical referral.

**Q: Can I track if my sleep treatment is working?**
Yes, the `evaluate_intervention_efficacy` tool calculates the percentage reduction in severity following an intervention.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/insomnia-severity-tracker](https://vinkius.com/en/ai-agent-connect/insomnia-severity-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Insomnia Severity Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `insomnia-severity-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Insomnia Severity Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "insomnia-severity-tracker": {
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
