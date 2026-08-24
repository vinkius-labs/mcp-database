# Legal Citation Formatter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/legal-citation-formatter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Converts raw legal citations into standardized formats for Bluebook, OSCOLA, AGLC, McGill, and ALWD.

## Description
This MCP server acts as a precision engine for legal professionals and researchers. It transforms unstructured legal text into perfectly formatted citations across five major global systems: The Bluebook (US), OSCOLA (UK), AGLC (Australia), McGill Guide (Canada), and ALWD (US). Using the `transform_citation` tool, you can convert raw case names, statutes, or journal references into precise, publication-ready strings. The engine handles complex requirements like reporter abbreviations, pinpoint page formatting, signal usage, and parallel citations. You can also use `validate_authority_type` to identify if a text represents a case, statute, journal, or treaty, and `resolve_parallel_citations` to ensure all required jurisdictional versions are present.


## Available Tools (3)
- **resolve_parallel_citations**: Identifies and reconciles multiple citation formats for a single authority
- **transform_citation**: Converts a raw, unstructured citation string into a structured set of formatted strings across all five target styles
- **validate_authority_type**: Analyzes a citation to determine if it represents a Case, Statute, Journal Article, or Treaty


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Legal Citation Formatter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Format this citation for Bluebook: Roe v. Wade 410 US 110"

**🤖 AI Agent:**
> Roe v. Wade, 410 U.S. 110 (1973).

---

**👤 You:**
> "What type of legal authority is '123 Stat. 456'?"

**🤖 AI Agent:**
> Statute

---

**👤 You:**
> "Format this for OSCOLA: R v Smith [2020] UKSC 15"

**🤖 AI Agent:**
> R v Smith [2020] UKSC 15


## ❓ FAQ

**Q: Which citation styles are supported?**
The server supports The Bluebook (21st ed.), OSCOLA (4th ed.), AGLC (4th ed.), McGill Guide (10th ed.), and ALWD (7th ed.).

**Q: Can I use short-form citations like 'Id.'?**
Yes. By providing the `contextualHistory` to the `transform_citation` tool, the engine can correctly apply short-form rules such as `Id.` or `Ibid.` based on the preceding citations.

**Q: How does the tool handle ambiguous citations?**
If a citation is too vague to be resolved deterministically, the `transform_citation` tool will return an `ambiguityFlag` set to true along with a reason explaining the uncertainty.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/legal-citation-formatter](https://vinkius.com/ai-agent-connect/legal-citation-formatter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Legal Citation Formatter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `legal-citation-formatter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Legal Citation Formatter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "legal-citation-formatter": {
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
