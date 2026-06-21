# Guidewire ClaimCenter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/guidewire-claimcenter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage insurance claims via ClaimCenter — track claim status, monitor exposures, and manage activities directly from any AI agent.

## Description
Connect your **Guidewire ClaimCenter** account to any AI agent and take full control of your insurance claims management through natural conversation. Streamline how you monitor and update claims natively.

### What you can do

- **Claim Oversight** — List and retrieve details for all active and historical insurance claims natively
- **Exposure Intelligence** — Access and monitor exposures associated with specific claims flawlessly
- **Activity Management** — List and review current activities and tasks across all claims securely
- **Document & Note Auditing** — List internal notes and uploaded documents for any claim flawlessly
- **User & Contact Logistics** — Access internal user rosters and shared contacts, including claimants and vendors, securely
- **Workflow Visibility** — Retrieve detailed claim metadata, policy numbers, and status updates directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ClaimCenter Cloud API Username, Password, and Instance URL
3. Start managing your insurance claims from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Claims Adjusters** — monitor claim status and review recent activities using natural language
- **Claims Managers** — audit exposure volumes and team task lists without opening the core application
- **Support Teams** — quickly look up claim details and policy references straight from their chat interface
- **Insurance Ops** — verify document uploads and note history during claim processing


## Available Tools
- **list_claim_activities**: List current activities and tasks across all claims
- **list_claimcenter_claims**: List insurance claims from Guidewire ClaimCenter
- **list_claim_contacts**: List shared contacts (claimants, vendors, providers)
- **list_claim_documents**: List uploaded documents for a specific claim
- **list_claim_exposures**: List exposures associated with a specific claim
- **list_claim_notes**: List internal notes for a specific claim
- **list_claimcenter_users**: List internal users and claim adjusters
- **get_claim_details**: Get detailed information for a specific claim


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Guidewire ClaimCenter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all claims with a status of 'Open' in ClaimCenter."

**🤖 AI Agent:**
> Retrieving your open claims... I found 5 items: Claim #000-01-0001 (Auto), #000-01-0002 (Property), and 3 others. Would you like to see the details for any of these?

---

**👤 You:**
> "Show me the exposures for claim '000-01-0001'."

**🤖 AI Agent:**
> Checking exposures for claim 000-01-0001... There are 2 active exposures: 1 for 'Vehicle Damage' (Adjuster: John Doe) and 1 for 'Liability' (Adjuster: Jane Smith).

---

**👤 You:**
> "Who is the primary contact for claim '000-01-0002'?"

**🤖 AI Agent:**
> Retrieving contacts for claim 000-01-0002... The primary contact is Mark Miller (Claimant). I can provide his phone number or email if needed.


## ❓ FAQ

**Q: Can I see the latest notes added to a specific claim?**
Yes! Use the `list_claim_notes` tool with the unique claim ID. The agent will return all internal notes associated with that claim, allowing you to catch up on recent updates.

**Q: How do I check the list of pending activities for the whole team?**
Use the `list_claim_activities` tool. Your agent will fetch all current tasks and activities across all claims, giving you a high-level view of the team's workload.

**Q: Where do I find my ClaimCenter Cloud API credentials?**
These credentials are provided by your Guidewire administrator. You will need a username and password with 'Cloud API' permissions, along with your organization's specific instance URL.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/guidewire-claimcenter](https://vinkius.com/mcp/guidewire-claimcenter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Guidewire ClaimCenter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `guidewire-claimcenter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Guidewire ClaimCenter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "guidewire-claimcenter": {
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
