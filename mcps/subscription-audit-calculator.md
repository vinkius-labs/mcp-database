# Subscription Audit Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/subscription-audit-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Audit subscription costs and identify wasted spending.

## Description
This MCP server provides tools to audit your subscription portfolio. Use `audit_subscriptions` to get a full summary of monthly costs, annual spending, and potential savings. You can also use `evaluate_single_subscription` for a granular look at a specific service's value, or `get_standard_benchmarks` to compare your costs against industry standards. It helps identify 'Overpriced' services based on your actual usage hours.


## Available Tools (3)
- **audit_subscriptions**: Audit subscriptions
- **evaluate_single_subscription**: Evaluate single subscription
- **get_standard_benchmarks**: Get benchmarks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Subscription Audit Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Audit my subscriptions: Netflix at 15.98 SGD for 10 hours, Spotify at 10.98 SGD for 20 hours, and my Gym at 100 SGD for 2 hours. My monthly income is 5000 SGD."

**🤖 AI Agent:**
> Your total monthly cost is 126.96 SGD. Your annual cost is 1523.52 SGD. Your Gym membership is 'Overpriced' due to high cost per hour. Your potential savings from canceling overpriced services is 100.00 SGD. Your subscription density is 2.54%.

---

**👤 You:**
> "Is my ChatGPT Plus subscription a good value? It costs 28 SGD and I use it for 30 hours a month."

**🤖 AI Agent:**
> Yes, ChatGPT Plus is a 'Good Value' with a cost of approximately 0.93 SGD per hour of use.

---

**👤 You:**
> "What are the standard costs for common subscriptions?"

**🤖 AI Agent:**
> Standard monthly costs include Netflix at 15.98 SGD, Spotify at 10.98 SGD, Disney+ at 11.98 SGD, YouTube Premium at 13.98 SGD, and ChatGPT Plus at 28.00 SGD.


## ❓ FAQ

**Q: How is the waste score calculated?**
The waste score is determined by dividing the monthly cost by your usage hours. If the cost per hour is greater than 5, it is marked as 'Overpriced'.

**Q: Can I compare my costs to standard prices?**
Yes, you can use the `get_standard_benchmarks` tool to retrieve standard monthly costs for common services like Netflix and Spotify.

**Q: What is subscription density?**
Subscription density is the percentage of your monthly income spent on subscriptions. A healthy density is typically below 5%.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/subscription-audit-calculator](https://vinkius.com/ai-agent-connect/subscription-audit-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Subscription Audit Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `subscription-audit-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Subscription Audit Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "subscription-audit-calculator": {
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
