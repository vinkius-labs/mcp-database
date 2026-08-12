# Template Injection Sanitizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/template-injection-sanitizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Detects and neutralizes prompt injection attacks using template syntax like Jinja2 and Python f-strings.

## Description
Protect your LLM applications from prompt injection attacks targeting template engines. This MCP server provides specialized tools to identify and remove malicious syntax used in frameworks like LangChain and CrewAI. Use `scan_input_security` to inspect individual strings for Jinja2 expressions, Python f-string patterns, or dangerous system variable access like `__class__`. For high-volume workloads, `batch_sanitize_inputs` allows for efficient bulk cleaning of user-generated content. This utility ensures that user inputs cannot manipulate prompt structures or leak sensitive data through interpolation.


## Available Tools (3)
- **batch_sanitize_inputs**: Processes a collection of strings to allow for bulk cleaning of user-generated content
- **get_injection_risk_profile**: Evaluates the severity of an injection attempt based on the density and type of patterns found
- **scan_input_security**: Analyzes a single input string to identify potential injection attempts and provides a cleaned version


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Template Injection Sanitizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this input is safe: 'Hello {{ user_name }}'"

**🤖 AI Agent:**
> The input contains a Jinja2 expression and has been flagged as injected.

---

**👤 You:**
> "Is this string malicious? 'print(obj.__class__)'"

**🤖 AI Agent:**
> The input contains system variable access and is considered a high-risk injection attempt.

---

**👤 You:**
> "Sanitize this list: ['safe text', '{secret_var}']"

**🤖 AI Agent:**
> The first item is safe, and the second item was sanitized by removing the Python f-string pattern.


## ❓ FAQ

**Q: What kind of injection attacks does this tool prevent?**
It prevents template-based prompt injection where attackers use Jinja2 or Python f-string syntax to manipulate LLM prompts or access system variables.

**Q: How do I check a single user input?**
You can use the `scan_input_security` tool to analyze a single string and receive a sanitized version along with a list of detected patterns.

**Q: Can I process multiple inputs at once?**
Yes, the `batch_sanitize_inputs` tool is designed to process a collection of strings efficiently in a single operation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/template-injection-sanitizer](https://vinkius.com/mcp/template-injection-sanitizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Template Injection Sanitizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `template-injection-sanitizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Template Injection Sanitizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "template-injection-sanitizer": {
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
