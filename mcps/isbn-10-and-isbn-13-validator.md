# ISBN-10 and ISBN-13 Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/isbn-10-and-isbn-13-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Verify the mathematical integrity of ISBN-10 and ISBN-13 identifiers and identify registration groups.

## Description
This MCP server provides precise mathematical validation for ISBN-10 and ISBN-13 identifiers. It can verify if a specific ISBN string is correct using `validate_isbn`, extract detailed formatting information with `get_isbn_metadata`, or identify the associated country or language group using `identify_registration_group`.


## Available Tools (3)
- **get_isbn_metadata**: Answers "What are the specific components and formatting details of this ISBN?"
- **identify_registration_group**: Answers "Which country or language group does this ISBN belong to?"
- **validate_isbn**: Answers "Is this specific ISBN string mathematically valid?"


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ISBN-10 and ISBN-13 Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the ISBN 0-306-40615-2 valid?"

**🤖 AI Agent:**
> Yes, 0-306-40615-2 is a valid ISBN-10.

---

**👤 You:**
> "What is the registration group for ISBN 978-3-16-148410-0?"

**🤖 AI Agent:**
> The ISBN 978-3-16-148410-0 belongs to the German registration group.

---

**👤 You:**
> "Give me the metadata for ISBN 9780545010221."

**🤖 AI Agent:**
> The ISBN 9780545010221 is an ISBN-13 with 13 digits.


## ❓ FAQ

**Q: How do I check if an ISBN is valid?**
You can use the `validate_isbn` tool by providing the raw ISBN string, including hyphens or spaces.

**Q: Can this tool identify the country of origin for a book?**
Yes, the `identify_registration_group` tool extracts the registration group prefix to determine the country or language group.

**Q: Does it support ISBN-10 with the 'X' check digit?**
Yes, the validation logic correctly handles the 'X' character used in ISBN-10 checksums.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/isbn-10-and-isbn-13-validator](https://vinkius.com/ai-agent-connect/isbn-10-and-isbn-13-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ISBN-10 and ISBN-13 Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `isbn-10-and-isbn-13-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ISBN-10 and ISBN-13 Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "isbn-10-and-isbn-13-validator": {
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
