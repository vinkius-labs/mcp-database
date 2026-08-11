# iCalendar Syntax Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/icalendar-syntax-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Validates iCalendar (ICS) structural integrity, component boundaries, and date-time syntax.

## Description
This MCP server provides precise validation for iCalendar (ICS) files. It ensures that components like VEVENT, VTODO, and VJOURNAL are correctly opened and closed, preventing structural failures. Use `validate_icalendar_structure` to check nesting, `verify_component_properties` to ensure mandatory fields like UID and DTSTAMP are present, and `check_date_time_syntax` to verify temporal formatting. It provides exact line numbers for any detected errors to facilitate rapid debugging.


## Available Tools (3)
- **check_date_time_syntax**: Scans the document to ensure all date and time properties follow the strict iCalendar temporal format
- **validate_icalendar_structure**: Checks the high-level structural integrity and nesting of the iCalendar string
- **verify_component_properties**: Validates that the required properties exist within specific component blocks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **iCalendar Syntax Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this ICS string structurally valid: 'BEGIN:VEVENT
UID:123
DTSTAMP:20230101T000000Z
END:VEVENT'"

**🤖 AI Agent:**
> Yes, the structure is valid and all mandatory properties are present.

---

**👤 You:**
> "Check if this VEVENT has the required UID and DTSTAMP properties."

**🤖 AI Agent:**
> The component is missing the required UID property.

---

**👤 You:**
> "Validate the date-time syntax in this string: 'BEGIN:VEVENT
DTSTART:2023-13-01
END:VEVENT'"

**🤖 AI Agent:**
> Syntax error detected: '2023-13-01' is an invalid date format.


## ❓ FAQ

**Q: What component types are supported?**
The validator specifically supports VEVENT, VTODO, and VJOURNAL components.

**Q: How can I find where an error occurred in my ICS file?**
The tools return the exact line number where the structural, property, or syntax error was detected.

**Q: Does this tool check for mandatory properties?**
Yes, you can use `verify_component_properties` to ensure that mandatory properties like UID and DTSTAMP are present in your components.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/icalendar-syntax-validator](https://vinkius.com/mcp/icalendar-syntax-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **iCalendar Syntax Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `icalendar-syntax-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **iCalendar Syntax Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "icalendar-syntax-validator": {
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
