# foundation-amount-total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/foundation-amount-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates aggregate foundation funding by analyzing application details and statuses.

## Description
This MCP server provides tools to manage and calculate foundation funding commitments. It allows users to retrieve specific details for an application using `get_application_details`, calculate total funding for specific statuses with `calculate_total_by_status`, list all submissions from an entity via `get_applications_by_applicant`, and check budget limits using `verify_funding_capacity`.


## Available Tools (4)
- **calculate_total_by_status**: g., "Approved") to calculate the total amount and count.

Calculate total funding committed to applications in a specific status
- **get_application_details**: Get specific details and funding amount of a single application
- **get_applications_by_applicant**: Get all applications submitted by a specific applicant
- **verify_funding_capacity**: Verify if current total requested funding is within a specific threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **foundation-amount-total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total funding for all Approved applications?"

**🤖 AI Agent:**
> The total funding committed to Approved applications is $500,000 across 12 applications.

---

**👤 You:**
> "Show me the details for application ID APP-123."

**🤖 AI Agent:**
> Application APP-123 was submitted by TechCorp for an amount of $50,000 and is currently in Pending status.

---

**👤 You:**
> "Is our current funding within a $1,000,000 limit?"

**🤖 AI Agent:**
> Yes, the current total is $750,000, leaving a remaining capacity of $250,000.


## ❓ FAQ

**Q: How can I see the total amount of approved grants?**
You can use the `calculate_total_by_status` tool and provide 'Approved' as the status to get the total amount and count.

**Q: Can I check if we have enough budget left for new applications?**
Yes, use the `verify_funding_capacity` tool by providing your maximum threshold to see the remaining capacity.

**Q: How do I find all applications for a specific organization?**
Use the `get_applications_by_applicant` tool and enter the name of the organization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/foundation-amount-total](https://vinkius.com/en/ai-agent-connect/foundation-amount-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **foundation-amount-total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `foundation-amount-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **foundation-amount-total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "foundation-amount-total": {
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
