# Household Emergency Contact Card Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-emergency-contact-card-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create printable emergency contact cards with prioritized contact sequences and language preferences.

## Description
This MCP server provides tools to organize and format critical household contact information into a ready-to-print emergency card. Use `generate_contact_card` to create a structured layout based on a specific contact order, or `validate_contact_data` to ensure all necessary details like phone numbers and addresses are present. You can also use `get_template_layout` to select different visual styles or `summarize_contact_list` to review your contact overview before printing.


## Available Tools (4)
- **summarize_contact_list**: Provides a high-level count and overview of the contacts provided
- **generate_contact_card**: Creates a formatted, printable text card containing all provided emergency contacts in a structured layout
- **get_template_layout**: Retrieves the visual structure/template for the card
- **validate_contact_data**: Checks the completeness and formatting of the contact information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Emergency Contact Card Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an emergency card for John Doe (555-0101, 123 Maple St, English) and Jane Doe (555-0102, 123 Maple St, English) with John as the primary contact."

**🤖 AI Agent:**
> EMERGENCY CONTACT CARD
----------------------
PRIMARY CONTACT:
Name: John Doe
Phone: 555-0101
Address: 123 Maple St
Language: English

SECONDARY CONTACT:
Name: Jane Doe
Phone: 555-0102
Address: 123 Maple St
Language: English

---

**👤 You:**
> "Check if my contact list is valid: [{'fullName': 'Alice', 'phoneNumber': '123', 'address': 'Road 1', 'preferredLanguage': 'en'}]"

**🤖 AI Agent:**
> The contact data is invalid because the phone number format is incorrect.

---

**👤 You:**
> "How many contacts are in this list: [{'fullName': 'Bob', 'phoneNumber': '555-1234', 'address': 'Street A', 'preferredLanguage': 'en'}, {'fullName': 'Charlie', 'phoneNumber': '555-5678', 'address': 'Street B', 'preferredLanguage': 'es'}]?"

**🤖 AI Agent:**
> You have provided 2 contacts. The languages used are English and Spanish.


## ❓ FAQ

**Q: How do I ensure the contacts are in the right order?**
You can use the `generate_contact_card` tool by providing a `contactOrder` array. This array should contain the names of your contacts in the exact sequence you want them to appear on the card.

**Q: What happens if I miss a phone number?**
The `validate_contact_data` tool will check your information. If a mandatory field like a phone number is missing, the validation will fail to ensure your emergency card is complete and reliable.

**Q: Can I change the look of the card?**
Yes, you can use `get_template_layout` to retrieve different visual structures, such as 'standard' or 'compact', to suit your needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-emergency-contact-card-generator](https://vinkius.com/en/ai-agent-connect/household-emergency-contact-card-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Emergency Contact Card Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-emergency-contact-card-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Emergency Contact Card Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-emergency-contact-card-generator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
