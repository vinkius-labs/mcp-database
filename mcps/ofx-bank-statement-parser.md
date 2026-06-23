# OFX Bank Statement Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ofx-bank-statement-parser)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Turn archaic OFX/QFX bank exports into clean JSON transactions safely and local. Let your AI act as your personal accountant without uploading sensitive financial data.

## Description
Nobody wants to upload their raw bank statement to a public cloud AI. But building a budget or calculating expenses manually is tedious. Furthermore, OFX and QFX files use an archaic SGML structure that completely confuses LLMs if they try to read the raw text directly.

This MCP acts as a secure, local financial bridge. It parses your bank's export file completely local, extracting only the clean transactional data (Date, Amount, Description, and Type) into a structured JSON array. The AI never sees the raw file, only the organized numbers, enabling it to act as your absolute best financial advisor.

### The Superpowers

- **100% Air-Gapped Privacy:** Your financial data is parsed locally on your machine. Zero cloud uploads.
- **Zero Hallucination:** The AI doesn't have to guess where a transaction begins and ends.
- **Universal Bank Support:** Works perfectly with any standard OFX or QFX file exported from global banks.
- **Accountant Ready:** Ask the AI: 'How much did I spend on Uber last month according to this file?'


## Available Tools (1)
- **parse_ofx_bank_statement**: Provide the absolute file path.

Parse an OFX or QFX bank statement file into clean JSON data. Extracts transactions safely and offline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OFX Bank Statement Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Read my statement.ofx and categorize all my expenses into a markdown table."

**🤖 AI Agent:**
> Here is your categorization:
| Category | Total Spent |
|---|---|
| Food & Dining | $450.00 |
| Transport | $120.00 |

---

**👤 You:**
> "Look at my bank export and find out exactly how much I paid to 'AWS' last year."

**🤖 AI Agent:**
> I found 12 transactions matching 'AWS' in your export, totaling exactly $1,450.32.

---

**👤 You:**
> "Analyze my monthly income versus expenses and calculate my savings rate."

**🤖 AI Agent:**
> Based on the OFX data, your total income was $5,000 and total expenses were $4,000. Your savings rate for this period is 20%.


## ❓ FAQ

**Q: Are my bank statements uploaded to Anthropic or OpenAI?**
Absolutely not. The parsing engine runs entirely on your local machine. It extracts the raw numbers and feeds them securely to the AI chat context window only during the session.

**Q: What exact data is extracted from the OFX?**
It extracts the bank ID, account ID, currency, and the full array of statement transactions including TRNTYPE, DTPOSTED, TRNAMT, FITID, NAME, and MEMO.

**Q: Can it process QFX files from Quicken?**
Yes! QFX is essentially the exact same structure as OFX. This engine reads both seamlessly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ofx-bank-statement-parser](https://vinkius.com/mcp/ofx-bank-statement-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OFX Bank Statement Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ofx-bank-statement-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OFX Bank Statement Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ofx-bank-statement-parser": {
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
