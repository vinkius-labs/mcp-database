# Rider Benefit Matcher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/rider-benefit-matcher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A precision logic engine that matches insurance rider clauses against loss events and expenses.

## Description
Rider Benefit Matcher connects AI agents to insurance policy logic. It evaluates verbatim rider text against specific loss scenarios and claimed expenses to identify guaranteed benefits and items requiring manual insurer adjudication. Use `analyze_rider_eligibility` to find explicit matches, `identify_document_requirements` to generate evidence checklists, `validate_expense_scope` to verify coverage, and `summarize_claim_status` for a high-level overview of guaranteed versus pending amounts.


## Available Tools (4)
- **analyze_rider_eligibility**: Determines which rider benefits are explicitly triggered by a loss event and its associated expenses
- **summarize_claim_status**: Provides a high-level overview of the claim's standing (Guaranteed vs. Pending)
- **identify_document_requirements**: Generates a specific checklist of documents needed to substantiate an identified benefit
- **validate_expense_scope**: Checks if a specific expense is even considered within the scope of the provided rider text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rider Benefit Matcher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this rider: 'Covers accidental dental injury up to $500'. Loss: A fall caused a chipped tooth. Expense: $300 for dental repair."

**🤖 AI Agent:**
> The dental repair expense is an explicit match under the accidental dental injury rider.

---

**👤 You:**
> "What documents do I need for a medical loss benefit?"

**🤖 AI Agent:**
> You will need to provide a Doctor's Statement and relevant medical receipts.

---

**👤 You:**
> "Is a $200 expense for 'emergency travel assistance' covered in a rider that only mentions 'accidental death'?"

**🤖 AI Agent:**
> No, the expense is not covered within the scope of the provided rider text.


## ❓ FAQ

**Q: How does the engine determine if a benefit is an explicit match?**
An explicit match occurs when the loss details satisfy the specific triggers in the rider text and the expense description aligns with the coverage scope.

**Q: What happens if a rider uses subjective language?**
If the rider contains subjective qualifiers like 'reasonable' or 'necessary', the item is flagged as requiring insurer confirmation.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, you can connect this MCP server to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/rider-benefit-matcher](https://vinkius.com/en/ai-agent-connect/rider-benefit-matcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rider Benefit Matcher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rider-benefit-matcher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rider Benefit Matcher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rider-benefit-matcher": {
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
