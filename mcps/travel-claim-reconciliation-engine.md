# Travel Claim Reconciliation Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/travel-claim-reconciliation-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Reconcile travel expenses with disruptions and insurance policies.

## Description
This MCP server provides a specialized engine to automate travel insurance claims. It uses `link_expenses_to_events` to correlate receipts with itinerary disruptions and policy rules, `identify_missing_documentation` to find gaps in evidence, `validate_claim_fields` to ensure compliance with insurer schemas, and `summarize_claim_status` to provide a high-level overview of claim readiness.


## Available Tools (4)
- **link_expenses_to_events**: Correlates individual expenses with specific itinerary disruptions and validates them against policy rules
- **summarize_claim_status**: Provides a high-level overview of the claim's progress, total value, and readiness
- **validate_claim_fields**: Ensures the final organized claim matches the specific data structure required by the insurance company's claim form
- **identify_missing_documentation**: Scans the results of the linking process to find valid expenses that lack sufficient evidence for a claim


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Travel Claim Reconciliation Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Link these expenses to the flight delay disruption."

**🤖 AI Agent:**
> The meal receipt for $25.00 has been successfully matched to the flight delay event on October 12th.

---

**👤 You:**
> "What is the current status of my travel claim?"

**🤖 AI Agent:**
> The claim has a total value of $150.00 with 2 matched expenses and 1 pending action for a missing hotel receipt.

---

**👤 You:**
> "Is my claim valid for the insurer's schema?"

**🤖 AI Agent:**
> The claim is valid and meets all required fields for submission.


## ❓ FAQ

**Q: How does the engine link expenses to disruptions?**
The `link_expenses_to_events` tool validates that the receipt timestamp falls within the disruption window and matches the policy terms.

**Q: What happens if I am missing a receipt?**
The `identify_missing_documentation` tool will flag the expense and provide a specific action to resolve the missing proof.

**Q: Can I check if my claim is ready to submit?**
Yes, you can use `summarize_claim_status` to see if the claim is 'Ready' based on matched expenses and missing actions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/travel-claim-reconciliation-engine](https://vinkius.com/en/ai-agent-connect/travel-claim-reconciliation-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Travel Claim Reconciliation Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `travel-claim-reconciliation-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Travel Claim Reconciliation Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "travel-claim-reconciliation-engine": {
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
