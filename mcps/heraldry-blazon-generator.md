# Heraldry Blazon Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/heraldry-blazon-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design](../categories/design.md)

Generates formal, grammatically correct heraldic blazons following strict Anglo-Norman rules.

## Description
This MCP server acts as a bridge between AI agents and the complex world of heraldry. It allows agents to convert visual shield components into formal, grammatically correct English blazon strings. By using tools like `generate_blazon`, agents can ensure they follow the strict Rule of Tincture (no metal on metal, no color on color) and proper syntax hierarchy (Field -> Ordinary -> Charges). It also provides specialized tools like `validate_tincture_pairing` to verify color combinations and `get_marshalling_description` to handle complex shield layouts like impalement or quartering.


## Available Tools (3)
- **generate_blazon**: Generates a complete, single-shield blazon string based on the provided visual components
- **get_marshalling_description**: Determines the correct heraldic terminology for combined arms (Impalement vs Quartering)
- **validate_tincture_pairing**: Checks if a specific combination of two tinctures is legally allowed under heraldic rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heraldry Blazon Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a blazon for a shield with a gold field and a red fess."

**🤖 AI Agent:**
> Or, a fess gules.

---

**👤 You:**
> "Create a blazon for a silver shield with a blue lion rampant."

**🤖 AI Agent:**
> Argent, a lion rampant azure.

---

**👤 You:**
> "What is the correct term for combining two arms vertically?"

**🤖 AI Agent:**
> The correct term for combining two arms vertically is impalement.


## ❓ FAQ

**Q: What is the Rule of Tincture?**
The Rule of Tincture is a fundamental heraldic principle stating that a metal (like Or or Argent) should not be placed upon another metal, and a color (like Gules or Azure) should not be placed upon another color, to ensure high visibility.

**Q: How do I generate a full description of a shield?**
You can use the `generate_blazon` tool by providing the field tincture, any divisions, ordinaries, and charges you wish to include.

**Q: Can this tool handle combined coats of arms?**
Yes, you can use `get_marshalling_description` to determine the correct terminology for combining arms through impalement or quartering.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/heraldry-blazon-generator](https://vinkius.com/ai-agent-connect/heraldry-blazon-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heraldry Blazon Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heraldry-blazon-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heraldry Blazon Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heraldry-blazon-generator": {
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
