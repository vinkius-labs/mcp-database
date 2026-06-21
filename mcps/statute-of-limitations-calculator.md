# Statute of Limitations Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/statute-of-limitations-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Determine legal expiration dates for various claims by applying statutory periods.

## Description
The Statute of Limitations Calculator is a specialized engine that calculates the exact calendar date on which a legal claim expires. By providing a legal domain (such as Labor, Civil, Tax, or Consumer) and a trigger date, you can use tools like `search_statutory_period` to find the duration of a claim, `calculate_deadline` to compute the expiration date, and `check_claim_validity` to assess if a claim is still active or has already expired. This tool helps legal professionals and individuals track critical deadlines for litigation.


## Available Tools (3)
- **calculate_deadline**: Compute the exact expiration date for a legal claim
- **check_claim_validity**: Check the viability of a claim
- **search_statutory_period**: Identify the specific duration and legal basis for a legal category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Statute of Limitations Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the statute of limitations for a Labor claim?"

**🤖 AI Agent:**
> The statutory period for Labor claims is 2 years.

---

**👤 You:**
> "If a consumer issue happened on 2023-01-01, when does it expire?"

**🤖 AI Agent:**
> The expiration date for this Consumer claim is 2024-01-01.

---

**👤 You:**
> "Is my Civil claim from 2020-05-20 still valid?"

**🤖 AI Agent:**
> No, the claim has expired.


## ❓ FAQ

**Q: What legal domains are supported?**
The calculator supports Labor, Civil, Tax, and Consumer law domains.

**Q: How do I calculate an expiration date?**
Use the `calculate_deadline` tool by providing the legal domain and the trigger date in ISO 8601 format.

**Q: Can I check if a claim is already expired?**
Yes, the `check_claim_validity` tool evaluates whether a claim is 'Active' or 'Expired' based on the provided date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/statute-of-limitations-calculator](https://vinkius.com/mcp/statute-of-limitations-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Statute of Limitations Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `statute-of-limitations-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Statute of Limitations Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "statute-of-limitations-calculator": {
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
