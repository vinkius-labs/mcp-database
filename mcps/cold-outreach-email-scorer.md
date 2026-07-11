# Cold Outreach Email Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cold-outreach-email-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Audit cold email effectiveness by scoring personalization, value proposition placement, and call-to-action clarity.

## Description
The Cold Outreach Email Scorer analyzes your sales emails to ensure high conversion rates. Use `evaluate_email_quality` to check if your personalization goes beyond simple name tokens and if your value proposition appears in the first two sentences. The `validate_cadence_pattern` tool helps you maintain professional follow-up intervals, while `check_subject_alignment` prevents clickbait by verifying that your subject line matches the email body content.


## Available Tools (2)
- **calculate_effectiveness_score**: Calculate the effectiveness score of an email
- **evaluate_email_quality**: Evaluate the quality of a cold outreach email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cold Outreach Email Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Evaluate this email: 'Hi Sarah, I loved your article on Kubernetes. We have a new cloud solution that might interest you. Let me know if you want to chat.' with context 'Sarah is a DevOps Engineer at TechCorp'."

**🤖 AI Agent:**
> The personalization depth is Deep because it references specific professional interests, and the value proposition placement is Immediate.

---

**👤 You:**
> "Check this follow-up cadence: [1, 4, 10]"

**🤖 AI Agent:**
> The cadence adherence is Optimal, as the intervals between touchpoints are within professional standards.

---

**👤 You:**
> "Does this subject line match? Subject: 'Quick question' Body: 'I wanted to discuss our enterprise pricing plans for next year.'"

**🤖 AI Agent:**
> The alignment score is Low. The subject line does not clearly communicate the topic of enterprise pricing mentioned in the body.


## ❓ FAQ

**Q: How does the tool measure personalization?**
The `evaluate_email_quality` tool checks for recipient-specific context in the email body beyond just using their name.

**Q: Can I check my follow-up sequence?**
Yes, use `validate_cadence_pattern` to ensure your touchpoints follow professional industry standards.

**Q: How do I avoid being flagged as clickbait?**
Use `check_subject_alignment` to confirm that the promise in your subject line is fulfilled within the email body.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cold-outreach-email-scorer](https://vinkius.com/mcp/cold-outreach-email-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cold Outreach Email Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cold-outreach-email-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cold Outreach Email Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cold-outreach-email-scorer": {
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
