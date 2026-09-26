# Family Photo Consent Register MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-photo-consent-register)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legal](../categories/legal.md)

Manage and track photographic usage permissions and consent status.

## Description
This MCP server provides a secure system for managing photographic likeness permissions. It allows users to `register_consent` for individuals, check current permissions via `get_consent_status`, search for historical records using `query_person_permissions`, and process formal revocations with `withdraw_consent`. It ensures that usage rights, durations, and withdrawal protocols are strictly maintained.


## Available Tools (4)
- **query_person_permissions**: Find all active and historical consent records associated with a specific individual
- **register_consent**: Create a new, legally binding consent record for an individual
- **withdraw_consent**: Process a formal request to revoke photographic permissions
- **get_consent_status**: Check if a specific person's consent is currently valid and what the limitations are


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Photo Consent Register** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Register consent for Jane Doe for social media and editorial use, starting today, with contact jane@example.com and instructions to email support to withdraw."

**🤖 AI Agent:**
> Consent registered successfully. Permission Reference: REF-12345. Status: active.

---

**👤 You:**
> "What is the current status of the consent for permission REF-12345?"

**🤖 AI Agent:**
> The consent for Jane Doe is currently active. Allowed uses: social media, editorial.

---

**👤 You:**
> "Find all consent records for John Smith."

**🤖 AI Agent:**
> Found 2 records for John Smith: REF-9876 (active) and REF-5432 (withdrawn).


## ❓ FAQ

**Q: How do I create a new consent record?**
You can use the `register_consent` tool to create a new record by providing the person's name, allowed uses, and contact details.

**Q: Can I revoke a permission that was previously granted?**
Yes, you can use the `withdraw_consent` tool to permanently revoke an existing permission using its unique reference ID.

**Q: How can I check if a specific consent is still valid?**
Use the `get_consent_status` tool with the permission reference to see if the status is active, withdrawn, or expired.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-photo-consent-register](https://vinkius.com/en/ai-agent-connect/family-photo-consent-register)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Photo Consent Register** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-photo-consent-register` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Photo Consent Register** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-photo-consent-register": {
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
