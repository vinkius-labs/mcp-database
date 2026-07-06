# Have I Been Pwned MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/have-i-been-pwned)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Check if your accounts or passwords have been compromised in data breaches using the HIBP service.

## Description
Connect your AI agent to **Have I Been Pwned**, the internet's most trusted resource for tracking data breaches. Protect yourself by staying informed about where your sensitive information may have been leaked.

### What you can do

- **Account Search** — Instantly check if an email or username has been involved in any of the thousands of tracked data breaches
- **Paste Search** — Discover if your information is circulating on public paste sites (like Pastebin)
- **Password Safety** — Safely verify if a password has ever appeared in a breach using the secure K-Anonymity model (your full password is never sent to the server)
- **Breach Catalog** — Explore the full history of major internet data breaches, including what types of data were stolen (passwords, emails, phone numbers, etc.)

### How it works

1. Subscribe to this server
2. Enter your **HIBP API Key** (available at [haveibeenpwned.com/API/Key](https://haveibeenpwned.com/API/Key))
3. Start auditing your digital safety through chat

### Who is this for?

- **Security-Conscious Users** — monitor personal or family accounts for leaks
- **IT Professionals** — check for corporate domain or account compromises
- **Researchers** — analyze trends and impact of major data breaches


## Available Tools (5)
- **search_account_breaches**: Search for all data breaches an email or account has been involved in
- **search_account_pastes**: Search for all public pastes (like Pastebin) containing the email or account
- **check_password_safety**: Uses k-anonymity; your full password is never sent to the server.

Check if a password has ever appeared in a data breach (safe, k-anonymity search)
- **get_breach_details**: Get details for a specific data breach by name
- **list_all_breaches**: List all data breaches currently recorded in the system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Have I Been Pwned** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Has my email 'test@example.com' been involved in any breaches?"

**🤖 AI Agent:**
> Checking breaches for 'test@example.com'... I found 3 breaches: Adobe (2013), LinkedIn (2016), and Canva (2019). Leaked data includes: Email addresses, Passwords, Usernames.

---

**👤 You:**
> "Is the password 'P@ssword123' safe to use?"

**🤖 AI Agent:**
> ⚠️ **DANGER!** This password has appeared in **45,210** data breaches. You should **NEVER** use this password as it is easily guessable and publicly known.


## ❓ FAQ

**Q: Is it safe to check my password using this tool?**
Yes. This agent uses the K-Anonymity model. Only the first 5 characters of your password's SHA-1 hash are sent to the HIBP server. The full password or full hash never leaves your local environment, making it cryptographically safe.

**Q: Where can I get an API Key?**
You can purchase an API key directly from the [HIBP website](https://haveibeenpwned.com/API/Key). It requires a small monthly subscription to prevent mass scraping and abuse.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/have-i-been-pwned](https://vinkius.com/mcp/have-i-been-pwned)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Have I Been Pwned** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `have-i-been-pwned` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Have I Been Pwned** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "have-i-been-pwned": {
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
