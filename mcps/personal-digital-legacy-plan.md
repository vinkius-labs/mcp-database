# Personal Digital Legacy Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/personal-digital-legacy-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize digital assets, access rights, and estate instructions with strict privacy controls.

## Description
This MCP server provides a structured framework for managing digital legacies. It helps users organize digital accounts, designate trusted contacts, and create secure storage plans for sensitive assets. Using tools like `generate_account_instruction_register`, `generate_trusted_contact_briefing`, `create_secure_storage_plan`, and `generate_annual_review_agenda`, you can ensure that your digital estate is handled according to your explicit authorization and the principle of least-disclosure. It is designed to bridge the gap between your digital life and your future executors or trusted contacts.


## Available Tools (4)
- **create_secure_storage_plan**: Maps the user's digital assets to a tiered security strategy
- **generate_account_instruction_register**: Provides a structured list of digital accounts and the specific actions/access rules associated with each
- **generate_annual_review_agenda**: Produces a checklist and schedule to ensure the legacy plan remains current
- **generate_trusted_contact_briefing**: Creates a curated information packet for a specific individual designated as a trusted contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personal Digital Legacy Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an instruction register for my Gmail and iCloud accounts."

**🤖 AI Agent:**
> Here is your account instruction register: Gmail (Type: Email, Instruction: Provide access to executor via recovery email), iCloud (Type: Cloud Storage, Instruction: Provide access to executor via master password).

---

**👤 You:**
> "Create a secure storage plan for my digital documents and master passwords."

**🤖 AI Agent:**
> Your secure storage plan is ready: Master Passwords are assigned to Vault Storage, and Digital Documents are assigned to Vault Storage.

---

**👤 You:**
> "What is the next step for my annual review if I last reviewed my plan on 2023-01-01?"

**🤖 AI Agent:**
> Your next scheduled review is 2024-01-01. Tasks include verifying your account list and validating your current trusted contacts.


## ❓ FAQ

**Q: How does this tool protect my privacy?**
The server follows the Least-Disclosure principle. For example, when using `generate_trusted_contact_briefing` with a minimal scope, contacts only receive location-based information rather than sensitive credentials.

**Q: Can I manage my digital assets for my heirs?**
Yes. You can use `generate_account_instruction_register` to create a structured list of accounts and specific instructions for your executors.

**Q: How often should I update my legacy plan?**
You can use `generate_annual_review_agenda` to produce a customized checklist and schedule to ensure your plan remains current and your trusted contacts are still valid.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/personal-digital-legacy-plan](https://vinkius.com/en/ai-agent-connect/personal-digital-legacy-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Personal Digital Legacy Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `personal-digital-legacy-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Personal Digital Legacy Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "personal-digital-legacy-plan": {
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
