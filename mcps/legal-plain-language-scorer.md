# Legal Plain Language Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/legal-plain-language-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze legal text for readability, syntax complexity, and defined term consistency.

## Description
The Legal Plain Language Scorer is a specialized tool designed to evaluate legal documents, terms of service, and contracts against plain-language standards. By connecting AI agents to linguistic metrics, it provides deep insights into text complexity. Use `evaluate_readability` to determine Flesch Reading Ease and Grade Level, `analyze_syntax` to detect passive voice density and nominalization, and `audit_definitions` to ensure capitalized terms are used consistently throughout your document.


## Available Tools (3)
- **analyze_syntax**: Analyze mechanical complexity in legal text
- **audit_definitions**: Audit consistency of defined terms in legal text
- **evaluate_readability**: Analyze the readability of legal text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Legal Plain Language Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How readable is this clause: 'The Company shall, at its sole discretion, implement the termination of the agreement.'?"

**🤖 AI Agent:**
> The text has a high nominalization density due to 'the termination of'. Using 'terminating the agreement' would improve readability.

---

**👤 You:**
> "Check if my defined terms are consistent in this text: 'The User agrees to the Terms. The user must follow rules.'"

**🤖 AI Agent:**
> Inconsistent term found: 'user' was used in lowercase after being defined as 'User'.

---

**👤 You:**
> "Analyze the syntax of this sentence: 'The implementation of the policy was performed by the committee.'"

**🤖 AI Agent:**
> This sentence contains passive voice ('was performed by') and high nominalization density ('the implementation of').


## ❓ FAQ

**Q: What metrics does this tool measure?**
It measures Flesch Reading Ease, Flesch-Kincaid Grade Level, passive voice ratio, sentence length distribution, nominalization density, and defined term consistency.

**Q: How can I check for inconsistent terms?**
Use the `audit_definitions` tool. It identifies capitalized terms defined at the start of your text and flags any subsequent lowercase usage.

**Q: Does this support large legal documents?**
Yes, the tool is designed to parse and analyze full bodies of legal text for structural and linguistic complexity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/legal-plain-language-scorer](https://vinkius.com/mcp/legal-plain-language-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Legal Plain Language Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `legal-plain-language-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Legal Plain Language Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "legal-plain-language-scorer": {
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
