# Disposable Email Blocker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/disposable-email-blocker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip Lead Gen AI Agents with throwaway email detection. Block fake emails instantly to protect your Sender Reputation.

## Description
When a Martech AI Agent reads a form submission from a user with the email `ceo@mailinator.com` or `admin@10minutemail.com`, the LLM has no idea it's a disposable email. If the agent triggers a welcome sequence, the email will bounce, damaging the client's SendGrid or Mailgun sender reputation. This MCP solves that perfectly.

### The Superpowers

- **Local Validation:** Uses a massive, community-maintained local JSON list of thousands of disposable domains to validate leads instantly.
- **Reputation Shield:** Allows Marketing Agents to definitively reject low-quality leads before inserting them into a CRM like Salesforce or HubSpot.


## Available Tools
- **check_disposable**: Pass the full email address and the engine checks the domain against a curated offline database of disposable email providers. Returns whether the email is disposable or legitimate.

Checks if an email belongs to a disposable or temporary email provider. Protects Sender Reputation for Martech AI Agents


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Disposable Email Blocker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this new lead's email `user@mailinator.com` is a throwaway address."

**🤖 AI Agent:**
> Disposable Email Validation: Domain is disposable. Action Recommended: BLOCK.

---

**👤 You:**
> "Is `ceo@vinkius.com` a legitimate corporate email?"

**🤖 AI Agent:**
> Disposable Email Validation: Domain is NOT disposable. Action Recommended: ALLOW.

---

**👤 You:**
> "Validate this CRM contact list item: `tester@10minutemail.com`."

**🤖 AI Agent:**
> Disposable Email Validation: Block action recommended.


## ❓ FAQ

**Q: Is this a network API request?**
No, it uses an local community-maintained list of domains. It runs perfectly in 0ms without hitting external endpoints.

**Q: Will it block Gmail or Outlook?**
No, legitimate global consumer providers like Gmail, Yahoo, and Outlook are strictly ignored by the blocklist.

**Q: What happens if a user submits a fake domain?**
The engine returns `isDisposable: true` and `actionRecommended: BLOCK`, allowing the agent to branch its logic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/disposable-email-blocker](https://vinkius.com/mcp/disposable-email-blocker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Disposable Email Blocker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `disposable-email-blocker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Disposable Email Blocker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "disposable-email-blocker": {
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
