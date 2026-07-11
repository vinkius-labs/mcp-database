# SMS Marketing Compliance Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sms-marketing-compliance-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Validate SMS marketing copy for encoding efficiency, regulatory compliance, and link optimization.

## Description
This MCP server provides a powerful engine to audit SMS campaigns. Use `analyze_encoding_impact` to detect if emojis or special characters will force a switch from GSM-7 to UCS-2 encoding, which increases segment costs. The `validate_regulatory_compliance` tool ensures your messages include mandatory opt-out keywords like "STOP" and "HELP", as well as proper sender identification. Additionally, use `calculate_link_optimization` to determine the character savings achieved by using shortened URLs in your campaigns.


## Available Tools (3)
- **analyze_encoding_impact**: Determine SMS encoding type and segment count
- **calculate_link_optimization**: Measure character savings from URL shortening
- **validate_regulatory_compliance**: Validate presence of required legal elements in SMS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SMS Marketing Compliance Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check this SMS for encoding issues: 'Hello! 👋 Check out our sale!'"

**🤖 AI Agent:**
> The message uses UCS-2 encoding due to the emoji. Total segments required: 2.

---

**👤 You:**
> "Is this message compliant? 'BrandX: Sale starts now! Text STOP to opt out.'"

**🤖 AI Agent:**
> Compliance check passed. Sender identification 'BrandX' and opt-out keyword 'STOP' were detected.

---

**👤 You:**
> "How many characters do I save if my URL is 100 chars and the short one is 25?"

**🤖 AI Agent:**
> You will save 75 characters, which is a 75% reduction in length.


## ❓ FAQ

**Q: How does the tool handle emojis?**
The `analyze_encoding_impact` tool detects if any character falls outside the GSM-7 set, triggering a UCS-2 encoding warning and calculating the increased segment count.

**Q: Can I check for legal compliance?**
Yes, use `validate_regulatory_compliance` to verify that your message contains required sender identification and opt-out instructions like "STOP" or "HELP".

**Q: Does it help with link shortening?**
Absolutely. The `calculate_link_optimization` tool calculates exactly how many characters you save by using a shortened URL compared to the original.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sms-marketing-compliance-checker](https://vinkius.com/mcp/sms-marketing-compliance-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SMS Marketing Compliance Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sms-marketing-compliance-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SMS Marketing Compliance Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sms-marketing-compliance-checker": {
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
