# Salesforce Service Cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salesforce-service-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage support cases, search the knowledge base, track case metrics, and resolve customer issues through natural conversation.

## Description
Connect **Salesforce Service Cloud** to any AI agent.

### What you can do
- **Cases** — Search, create, update, and filter by status or priority
- **Comments** — Read and add internal/public case comments
- **Knowledge** — Search published knowledge articles for instant answers
- **Metrics** — Aggregate case counts by status and priority

### Who is this for?
- **Support Agents** — Resolve tickets without opening Salesforce
- **CS Managers** — Get instant support queue health checks
- **Success Teams** — Look up case history for any customer


## Available Tools
- **sf_add_case_comment**: Set isPublished to true if the comment should be visible to the customer (e.g., in a customer portal). Default is internal-only. Use to log agent responses, internal notes, or resolution steps on a support case.

Add a comment to a Salesforce case — internal note or customer-visible response
- **sf_create_case**: Subject is required. Status defaults to "New". Priority: High, Medium, Low. Origin: Web, Phone, Email. Link to a customer via contactId and their company via accountId (both use 18-char Salesforce IDs). Cases track the complete lifecycle of a customer support issue.

Create a new support case in Salesforce Service Cloud with subject, description, priority, origin, and linked contact/account
- **sf_case_comments**: Returns comment body, whether it is published (customer-visible), creator name, and creation date. Comments provide the full conversation history of a support case. Use to review case discussions or get context before responding.

Get all comments (internal and customer-visible) on a specific Salesforce case for case history review
- **sf_case_metrics**: Returns summary data: how many cases at each status × priority intersection. Perfect for support team dashboards, capacity planning, and identifying volume trends. Use when the user asks "how many open cases do we have?" or "what is the case breakdown by priority?"

Get aggregate support case metrics — case counts grouped by status and priority for a team dashboard view
- **sf_cases_by_status**: Returns cases sorted by priority then creation date. Use for support queue management: "how many new cases are there?", "show escalated cases", or for case workload analysis by status.

Get all Salesforce cases at a specific status for queue analysis — New, Working, Escalated, or Closed
- **sf_search_cases**: Returns case number, subject, status (New/Working/Escalated/Closed), priority (High/Medium/Low), origin channel (Web/Phone/Email), case owner, and description. Use when the user wants to find a specific support case, look up a case number, or review customer issues.

Search Salesforce Service Cloud cases by subject or case number to find customer support issues
- **sf_search_knowledge**: Returns article title, summary, URL, and article type. Salesforce Knowledge is the built-in KB for self-service and agent-assist. Use when the user asks for help articles, documented solutions, or wants to check if an issue has been addressed in the knowledge base.

Search the Salesforce Knowledge Base for published articles to find documented solutions and answers
- **sf_update_case**: Common operations: advance Status from "New" to "Working" to "Closed", escalate Priority to "High", or append to Description. Only specified fields change.

Update a Salesforce case — change status, escalate priority, or add description to reflect case progress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salesforce Service Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many open P1 cases do we have?"

**🤖 AI Agent:**
> 🎟️ **Open Case Metrics**

| Status | Priority | Count |
|---|---|---|
| New | High | 3 |
| Working | High | 7 |
| Escalated | High | 2 |

⚠️ **12 high-priority cases** currently open

---

**👤 You:**
> "Find a knowledge article about password reset"

**🤖 AI Agent:**
> 📚 Found 3 articles:
1. **How to Reset Your Password** — Step-by-step guide
2. **Password Policy FAQ** — Requirements and best practices
3. **Two-Factor Authentication Setup** — Adding extra security

---

**👤 You:**
> "Create a high-priority case: Login page returning 500 error"

**🤖 AI Agent:**
> ✅ **Case Created!**
- Subject: Login page returning 500 error
- Priority: High
- Status: New
- Origin: Web


## ❓ FAQ

**Q: What types of cases can I manage?**
All Salesforce Case records — filter by status (New, Working, Escalated, Closed), priority (High, Medium, Low), and origin (Web, Phone, Email).

**Q: Can I search the Knowledge Base?**
Yes! Searches published Knowledge articles by keyword and returns title, summary, and direct link.

**Q: Can I add comments to cases?**
Yes — add internal notes or customer-visible comments to any case.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesforce-service-cloud](https://vinkius.com/mcp/salesforce-service-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salesforce Service Cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `salesforce-service-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salesforce Service Cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salesforce-service-cloud": {
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
