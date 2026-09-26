# Family Insurance Contact Sheet MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-insurance-contact-sheet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Aggregates insurance policies, covered people, provider contacts, and claim history into a single dashboard.

## Description
This MCP server provides a unified interface to manage and view family insurance information. It connects AI agents to critical insurance data, allowing for quick retrieval of coverage summaries, provider contact details, specific policy administrative information, and claim histories. Use `get_coverage_summary` to see what an individual is covered for, `get_provider_directory` to find company contact info, `get_policy_details` to check renewal dates and covered people, and `track_claims` to review claim status and documentation.


## Available Tools (4)
- **get_coverage_summary**: Provides a high-level overview of all active insurance coverage for a specific person
- **get_policy_details**: Retrieves full administrative details for a specific insurance policy
- **get_provider_directory**: Lists all insurance providers and their contact information
- **track_claims**: Retrieves a history of claims associated with a specific policy or person


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Insurance Contact Sheet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What insurance does John Doe have?"

**🤖 AI Agent:**
> John Doe has two active policies: a Life Insurance policy (Policy #12345) and a Health Insurance policy (Policy #67890).

---

**👤 You:**
> "Find the contact details for BlueShield."

**🤖 AI Agent:**
> BlueShield can be reached at 555-0199 or via email at support@blueshield.com. Their website is https://www.blueshield.com.

---

**👤 You:**
> "Show me the claim history for policy #98765."

**🤖 AI Agent:**
> There is one claim recorded for policy #98765: Claim ID #CLM-001, which is currently in 'Processed' status.


## ❓ FAQ

**Q: How can I see all insurance coverage for a specific family member?**
You can use the `get_coverage_summary` tool by providing the person's full name to see their active policies.

**Q: Where can I find the contact information for my insurance provider?**
Use the `get_provider_directory` tool to list all known providers and their contact details, or filter by a specific company name.

**Q: How do I check when a policy is due for renewal?**
Provide the policy number to the `get_policy_details` tool to retrieve the renewal date and other administrative details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-insurance-contact-sheet](https://vinkius.com/en/ai-agent-connect/family-insurance-contact-sheet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Insurance Contact Sheet** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-insurance-contact-sheet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Insurance Contact Sheet** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-insurance-contact-sheet": {
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
