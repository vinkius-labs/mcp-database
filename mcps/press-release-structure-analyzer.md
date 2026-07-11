# Press Release Structure Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/press-release-structure-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [journalism](../categories/journalism.md)

Validates press release structure: inverted-pyramid check, quote density, and AP style compliance.

## Description
The Press Release Structure Analyzer ensures your news announcements adhere to professional journalistic standards. Using tools like `verify_lead_elements`, `validate_structural_formatting`, and `audit_quote_standards`, it checks for the presence of the Five W's, validates headline length against AP style guidelines, and audits quote density and attribution completeness.


## Available Tools (3)
- **audit_quote_standards**: Checks for appropriate quote density and attribution completeness
- **validate_structural_format**: Validates headline, dateline, and boilerplate formatting
- **verify_lead_elements**: Determines if a lead paragraph contains all critical news pillars


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Press Release Structure Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this press release lead is complete: 'Apple announced today in Cupertino that the new iPhone is coming.'"

**🤖 AI Agent:**
> The lead is missing the 'Why' element. It identifies Who (Apple), What (new iPhone), When (today), and Where (Cuperino), but not Why.

---

**👤 You:**
> "Is this headline valid? 'Breaking News: Massive Storm Hits New York City and Causes Widespread Damage Across the Five Boroughs Today!'"

**🤖 AI Agent:**
> The headline is invalid because it exceeds the 100-character limit.

---

**👤 You:**
> "Analyze this quote: 'We are excited,' said John Doe, CEO of TechCorp."

**🤖 AI Agent:**
> The attribution is complete, containing Name (John Doe), Title (CEO), and Company (TechCorp).


## ❓ FAQ

**Q: What does the tool check for in a lead paragraph?**
It uses `verify_lead_elements` to ensure the Who, What, When, Where, and Why are all present.

**Q: How is headline length validated?**
The `validate_structural_formatting` tool checks that the headline does not exceed 100 characters per AP style.

**Q: Can it check for proper quote attribution?**
Yes, `audit_quote_standards` verifies that quotes include the speaker's name, title, and company.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/press-release-structure-analyzer](https://vinkius.com/mcp/press-release-structure-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Press Release Structure Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `press-release-structure-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Press Release Structure Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "press-release-structure-analyzer": {
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
