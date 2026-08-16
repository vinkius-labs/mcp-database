# Email Header Metadata Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/email-header-metadata-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Extracts precise headers, hop counts, and domain information from raw RFC 822 email source text.

## Description
This MCP server provides deep visibility into email structures. By using the `extract_email_metadata` tool, you can parse raw RFC 822 email source text to identify critical headers such as From, To, Subject, Date, Message-ID, Received, and DKIM-Signature. It also calculates the exact hop count by analyzing 'Received:' headers and identifies domain names through strict regex parsing.


## Available Tools (1)
- **extract_email_metadata**: Parses raw RFC 822 email source text to extract metadata like headers, hop count, and domains


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Email Header Metadata Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you extract the metadata from this email source: 'From: alice@vinkius.com\nTo: bob@vinkius.com\nSubject: Hello\n\nHi Bob!'"

**🤖 AI Agent:**
> The email was sent from alice@vinkius.com to bob@vinkius.com with the subject 'Hello'.

---

**👤 You:**
> "How many hops did this email take? Source: 'Received: from host1\nReceived: from host2\nFrom: user@vinkius.com'"

**🤖 AI Agent:**
> This email took 2 hops.

---

**👤 You:**
> "Extract the domain from this email: 'From: sender@vinkius.com'"

**🤖 AI Agent:**
> The domain is vinkius.com.


## ❓ FAQ

**Q: What kind of email data can be extracted?**
The `extract_email_metadata` tool extracts standard headers like From, To, Subject, Date, Message-ID, Received, and DKIM-Signature, along with hop counts and domain names.

**Q: How is the hop count calculated?**
The hop count is determined by counting the number of 'Received:' header entries present in the raw email source.

**Q: Does this work with any email format?**
This tool is specifically designed for raw RFC 822 email source text.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/email-header-metadata-extractor](https://vinkius.com/ai-agent-connect/email-header-metadata-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Email Header Metadata Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `email-header-metadata-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Email Header Metadata Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "email-header-metadata-extractor": {
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
