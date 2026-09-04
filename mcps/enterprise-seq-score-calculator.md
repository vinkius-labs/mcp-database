# Enterprise SEQ Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-seq-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [crm](../categories/crm.md)

Measure sales engagement effectiveness using the SEQ methodology.

## Description
This MCP server provides tools to calculate the Sales Engagement Quality (SEQ) score, a metric designed to evaluate the meaningfulness of sales interactions. Instead of focusing on volume, it analyzes the impact of outreach on the sales pipeline. Use `get_seq_score` to evaluate overall engagement health, `get_engagement_efficiency` to determine if outreach is precise or noisy, `get_activity_mix_analysis` to ensure a balanced touchpoint strategy, and `get_optimization_roadmap` to receive actionable advice for improving engagement quality.


## Available Tools (4)
- **get_seq_score**: Calculates the primary SEQ score for a specific sales engagement
- **get_activity_mix_analysis**: Evaluates the variety of touchpoints to ensure engagement is not one-dimensional
- **get_engagement_efficiency**: Analyzes the relationship between activity volume and response rates
- **get_optimization_roadmap**: Provides actionable advice based on specific engagement gaps


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise SEQ Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the SEQ score for prospect P123 with 5 meetings, 20 emails, 3 content shares, 4 responses, deal progression true, and positive response quality."

**🤖 AI Agent:**
> The SEQ score for prospect P123 is 85. Your engagement is highly effective due to high response quality and successful deal progression.

---

**👤 You:**
> "Analyze the engagement efficiency for prospect P456 with 50 emails, 2 responses, and 1 meeting."

**🤖 AI Agent:**
> The efficiency rating is Low. Your touch density is high, indicating noisy outreach with a low response rate.

---

**👤 You:**
> "What is the activity mix for 10 emails, 0 content shares, and 2 meetings?"

**🤖 AI Agent:**
> The balance score is 45. Your primary channel is email, but you lack diversity in your touchpoints.


## ❓ FAQ

**Q: What is the SEQ score?**
The SEQ score is a normalized metric between 0 and 100 that represents the overall health and effectiveness of a sales engagement sequence.

**Q: How can I improve my engagement efficiency?**
You can use the `get_optimization_roadmap` tool to receive specific, actionable advice based on your current SEQ score and response quality.

**Q: Does this tool account for different types of sales activities?**
Yes, the `get_activity_mix_analysis` tool evaluates the balance between emails, content shared, and meetings held to ensure a diverse engagement strategy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-seq-score-calculator](https://vinkius.com/ai-agent-connect/enterprise-seq-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise SEQ Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-seq-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise SEQ Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-seq-score-calculator": {
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
