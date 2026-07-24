# ICU MessageFormat Validator Alternative MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/icu-messageformat-validator-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

A deterministic validator for ICU MessageFormat strings to prevent i18n breakage from unbalanced braces or incorrect syntax.

## Description
The ICU MessageFormat Validator is a specialized utility designed to ensure the structural integrity of internationalization strings. By implementing a deterministic finite automaton (DFA), the server performs deep analysis of message content to identify critical errors that break translation logic. The `validate_structural_braces` tool tracks brace depth and single-quote escaping states, specifically detecting unmatched '{' or '}' characters and unescaped quotes that would otherwise corrupt the interpolation engine. Additionally, the `validate_category_logic` tool verifies that all identifiers within plural and select blocks belong to the approved set of categories like zero, one, two, few, many, and other, ensuring the 'other' category is always present. For developers needing to identify dynamic content, the `extract_template_variables` tool parses strings to reveal all unique variable names used in the template, providing a clear inventory of required interpolation parameters.


## Available Tools (3)
- **validate_category_logic**: Validate the logic within plural/select blocks
- **extract_template_variables**: }`.

Extract template variables from an ICU message
- **validate_structural_braces**: Validate the structural integrity of braces and quotes in an ICU message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ICU MessageFormat Validator Alternative** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this ICU string is valid: '{name} has {count, plural, one {# message} other {# messages}}'"

**🤖 AI Agent:**
> The string is structurally sound. The `validate_structural_balances` tool confirms that all braces are paired and the plural categories are correct.

---

**👤 You:**
> "What variables are in this message: 'Hello {user}, you have {items} items.'"

**🤖 AI Agent:**
> The extracted variables are: user, items.

---

**👤 You:**
> "Is this string broken: '{unclosed_brace'"

**🤖 AI Agent:**
> No, the string is invalid. The `validate_structural_braces` tool detected an unmatched opening brace at the start of the string.


## ❓ FAQ

**Q: How does the validator handle single quotes?**
The `validate_structural_braces` tool implements a state machine to track escaping. It recognizes that two consecutive single quotes (double-single-quote) represent a literal single quote, preventing the parser from incorrectly terminating an escaped sequence.

**Q: What happens if I use an invalid category in a plural block?**
If you include an unsupported keyword like 'none' or 'all', the `validate_category_logic` tool will flag a syntax error, identifying the exact character offset where the invalid category was detected.

**Q: Can I use this to find all variables in my translation files?**
Yes, by using the `extract_template_variables` tool, you can provide any ICU string and receive a complete list of all unique variable names found within the template, such as 'userName' or 'itemCount'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/icu-messageformat-validator-alternative](https://vinkius.com/mcp/icu-messageformat-validator-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ICU MessageFormat Validator Alternative** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `icu-messageformat-validator-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ICU MessageFormat Validator Alternative** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "icu-messageformat-validator-alternative": {
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
