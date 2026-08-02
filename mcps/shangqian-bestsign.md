# ShangQian / 上上签 (BestSign) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shangqian-bestsign)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

China's leading digital signature platform — manage contracts, register users, and automate signatures via AI.

## Description
Empower your AI agent to orchestrate your digital document workflows and electronic signatures with **ShangQian** (BestSign / 上上签), the premier B2B digital signature platform in China. By connecting ShangQian to your agent, you transform complex contract lifecycle management, user identity verification (KYC), and signature orchestration into a natural conversation. Your agent can instantly register new personal or enterprise users, initialize contracts from pre-defined templates, retrieve detailed contract statuses, and even generate secure download links for executed documents without you ever needing to navigate the comprehensive BestSign Management Portal. Whether you are automating HR onboarding or coordinating high-volume commercial agreements, your agent acts as a real-time contract coordinator, providing accurate and fast results from a single, authorized source.

### What you can do

- **User Orchestration** — Register new users, verify digital certificates, and perform KYC identity checks.
- **Contract Management** — Create signature-ready contracts using templates and monitor real-time completion status.
- **Template Automation** — List and audit your library of contract templates and upload new document definitions.
- **Execution Control** — Trigger signature operations for authorized accounts and retrieve finalized PDF documents.
- **Operational Monitoring** — Verify API connectivity and monitor system health to ensure signature reliability.

### How it works

1. Subscribe to this server
2. Enter your ShangQian Developer ID and RT Secret
3. Start managing your digital signatures through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal & Compliance Teams** — automate contract status tracking and identity auditing through natural language.
- **HR & Operations** — coordinate employee onboarding and commercial agreement signing directly from your workspace.
- **Developers** — integrate professional-grade digital signature APIs into your AI-driven daily routines.
- **BestSign Power Users** — integrate your existing signature projects into your AI-driven daily routines.


## Available Tools (8)
- **create_shangqian_contract**: Create signature contract
- **get_contract_details**: Get contract metadata
- **get_contract_download**: Get download URL
- **get_user_certificate**: Get user certificate
- **register_shangqian_user**: Register a new user
- **sign_contract_now**: Sign contract
- **upload_shangqian_template**: Upload new template
- **verify_identity_v2**: Verify user identity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ShangQian / 上上签 (BestSign)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all contract templates in my ShangQian account."

**🤖 AI Agent:**
> I've retrieved your template list. You have 5 active templates, including 'Standard_Employment_Contract' (ID: `tem_8821`) and 'NDA_v2'. Would you like me to initialize a new contract using one of these?

---

**👤 You:**
> "Register a new enterprise user 'Vinkius' with account 'vinkius@example.com'."

**🤖 AI Agent:**
> I've successfully registered 'Vinkius' as an enterprise user in the ShangQian system. The account is now ready for digital certificate issuance and signing. Should I retrieve the certificate details?

---

**👤 You:**
> "What is the status of contract '88210934'?"

**🤖 AI Agent:**
> Contract `88210934` ('Sales Agreement') is currently 'PARTIALLY_SIGNED'. 1 out of 2 signers have completed their signatures. Would you like me to generate a download link for the current draft?


## ❓ FAQ

**Q: How do I find my ShangQian Developer ID and Secret?**
Log in to the [BestSign Developer Platform](https://open.bestsign.cn/), navigate to the 'Application Management' or 'Credentials' section to find your unique Developer ID and RT Secret.

**Q: What is the 'account' identifier?**
The account identifier is a unique string used to identify a user in the ShangQian system, typically a mobile phone number or an email address. It is required for registration and signing operations.

**Q: Does this server handle HMAC-SHA1 signatures?**
Yes! The server automatically calculates the required HMAC-SHA1 signature using your RT Secret for every request, ensuring secure authorized communication with the ShangQian API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shangqian-bestsign](https://vinkius.com/mcp/shangqian-bestsign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ShangQian / 上上签 (BestSign)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shangqian-bestsign` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ShangQian / 上上签 (BestSign)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shangqian-bestsign": {
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
