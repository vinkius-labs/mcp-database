# Renewal Comparison Brief MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/renewal-comparison-brief)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare insurance policy terms and generate renewal decision briefs.

## Description
This MCP server provides specialized tools for insurance professionals to evaluate renewal offers. Use `analyze_policy_discrepancies` to identify shifts in premiums, limits, and deductibles between current and renewal policies. Generate structured narratives with `generate_decision_brief` and formulate strategic inquiries for brokers using `generate_insurer_questions`. You can also ensure compliance with `validate_policy_alignment` to verify that renewal offers meet your minimum coverage requirements.


## Available Tools (4)
- **analyze_policy_discrepancies**: Identifies and quantifies the differences between the current policy and the renewal offer for matching coverage types
- **generate_decision_brief**: Produces a structured narrative summarizing the financial and coverage-based implications of the renewal
- **generate_insurer_questions**: Formulates specific, professional questions intended to be sent to the insurance broker or carrier
- **validate_policy_alignment**: Checks if the renewal offer maintains the minimum required coverage levels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Renewal Comparison Brief** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these two policies and tell me the main differences in premium and limits."

**🤖 AI Agent:**
> The premium has increased by $500, while the coverage limits remain unchanged at $1,000,000.

---

**👤 You:**
> "Does this renewal offer meet my minimum requirement of a $500 deductible?"

**🤖 AI Agent:**
> No, the renewal offer has a deductible of $1,000, which exceeds your maximum requirement of $500.

---

**👤 You:**
> "Generate questions for the insurer regarding the increased premium."

**🤖 AI Agent:**
> Could you please provide a detailed justification for the premium increase, given that the coverage limits and deductibles have not changed?


## ❓ FAQ

**Q: How do I compare my current policy with a renewal offer?**
You can use the `analyze_policy_discrepancies` tool by providing the JSON representations of both your current policy and the renewal offer.

**Q: Can I generate questions for my insurance broker?**
Yes, the `generate_insurer_questions` tool creates professional questions based on the discrepancies found during analysis.

**Q: How can I check if a renewal meets my minimum coverage needs?**
Use the `validate_policy_alignment` tool to compare the renewal offer against your specific minimum requirements for limits and deductibles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/renewal-comparison-brief](https://vinkius.com/en/ai-agent-connect/renewal-comparison-brief)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Renewal Comparison Brief** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `renewal-comparison-brief` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Renewal Comparison Brief** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "renewal-comparison-brief": {
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
