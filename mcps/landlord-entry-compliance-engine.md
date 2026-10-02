# Landlord Entry & Compliance Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/landlord-entry-compliance-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [property-management](../categories/property-management.md)

Audits landlord entry requests against lease rules, tenant availability, and calendar conflicts.

## Description
This MCP server provides a compliance and scheduling validation engine for property management. It allows AI agents to audit entry requests by checking them against lease-specified notice periods and permitted purposes using `get_entry_compliance`. It can verify if a requested time aligns with tenant schedules via `check_tenant_availability` and identify overlapping appointments with `detect_calendar_conflicts`. Finally, it can aggregate all data into a single view using `generate_compliance_report` to identify compliant visits, notice violations, and schedule conflicts.


## Available Tools (4)
- **check_tenant_availability**: Check availability
- **detect_calendar_conflicts**: Detect conflicts
- **generate_compliance_report**: Generate report
- **get_entry_compliance**: Audit entry request


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Landlord Entry & Compliance Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the entry request for notice ID 123 compliant with the lease?"

**🤖 AI Agent:**
> No, the entry request for notice ID 123 is marked as 'Insufficient Notice' because the requested entry date is only 24 hours after the notice was issued, violating the 48-hour lease requirement.

---

**👤 You:**
> "Check if the tenant is available for a maintenance visit on 2024-08-15 between 10:00 and 12:00."

**🤖 AI Agent:**
> The tenant is available during the requested window on 2024-08-15 from 10:00 to 12:00.

---

**👤 You:**
> "Are there any calendar conflicts for property ID prop_987 on 2024-09-01 from 14:00 to 16:00?"

**🤖 AI Agent:**
> Yes, there is a conflict. A scheduled plumbing repair is already set for 2024-09-01 from 15:00 to 16:00.


## ❓ FAQ

**Q: How does the tool determine if a notice is sufficient?**
The `get_entry_compliance` tool compares the time between the notice issuance and the requested entry against the mandatory notice period defined in the property's lease agreement.

**Q: Can I check for scheduling conflicts?**
Yes, you can use `detect_calendar_conflicts` to see if a proposed entry window overlaps with existing scheduled activities in the property calendar.

**Q: What information is needed for a compliance report?**
To use `generate_compliance_report`, you need to provide the property identifier and the start and end dates for the reporting period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/landlord-entry-compliance-engine](https://vinkius.com/en/ai-agent-connect/landlord-entry-compliance-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Landlord Entry & Compliance Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `landlord-entry-compliance-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Landlord Entry & Compliance Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "landlord-entry-compliance-engine": {
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
