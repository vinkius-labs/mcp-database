# Insurance Policy Record Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/insurance-policy-record-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A secure system for managing insurance policies, renewal schedules, and claim documentation.

## Description
This MCP server provides a centralized management system for organizing insurance policy details. It allows AI agents to access a secure policy register, generate document folder maps, view a review calendar for upcoming renewals, and verify claim-readiness for specific assets. Use `get_policy_register` to view policy summaries, `get_document_map` to locate files, `get_review_calendar` to track audit dates, and `check_claim_readiness` to ensure all necessary documentation is prepared for a claim.


## Available Tools (4)
- **check_claim_readiness**: Evaluates if a specific policy and its covered assets have all necessary documentation
- **get_document_map**: Generates a structured view of where specific policy documents are located
- **get_policy_register**: You can filter by privacy level.

Provides a secure, high-level summary of all managed insurance policies
- **get_review_calendar**: Retrieves a schedule of upcoming policy audits based on renewal dates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Insurance Policy Record Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a summary of my public insurance policies."

**🤖 AI Agent:**
> Here is the summary of your public insurance policies: Policy ID: POL-123, Type: Auto, Insurer: SafeDrive, Expiry: 2025-05-20, Status: Active.

---

**👤 You:**
> "Where are the documents for policy POL-987 stored?"

**🤖 AI Agent:**
> The documents for policy POL-987 are located in the following paths: Proof of Ownership: /storage/docs/POL-987/ownership.pdf, Asset Appraisal: /storage/docs/POL-987/appraisal.pdf.

---

**👤 You:**
> "Is my property insurance (POL-456) ready for a claim on asset ASSET-001?"

**🤖 AI Agent:**
> Yes, the documentation for asset ASSET-001 under policy POL-456 is complete and ready for submission.


## ❓ FAQ

**Q: How does the system handle sensitive policy information?**
The system uses privacy categorization to assign sensitivity tiers. You can use `get_policy_register` with specific privacy levels to ensure only authorized information is retrieved.

**Q: How can I know if I am ready to file a claim?**
You can use the `check_claim_readiness` tool to evaluate if all required documents for a specific asset are organized and verified.

**Q: How are renewal alerts managed?**
Renewal alerts are managed via a review calendar. By using `get_review_calendar`, you can see a schedule of upcoming audits based on policy lead-time rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/insurance-policy-record-plan](https://vinkius.com/en/ai-agent-connect/insurance-policy-record-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Insurance Policy Record Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `insurance-policy-record-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Insurance Policy Record Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "insurance-policy-record-plan": {
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
