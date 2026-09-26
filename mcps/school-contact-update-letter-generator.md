# School Contact Update Letter Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/school-contact-update-letter-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Generates formal school notification letters for student contact updates.

## Description
This MCP server provides a suite of tools to automate the creation of professional school correspondence. It allows administrators to generate send-ready notification letters whenever a student's contact information is modified. Using `generate_update_letter`, you can produce a complete letter that highlights specific changes between old and new contact details. The server also includes `validate_contact_delta` to identify changes, `format_student_header` for standardized administrative headers, and `check_delivery_constraints` to ensure delivery methods meet regional requirements.


## Available Tools (4)
- **validate_contact_delta**: Analyzes the difference between two contact sets to identify specifically what changed
- **check_delivery_constraints**: Verifies if the requested delivery method is valid for the specified region
- **format_student_header**: Generates the standardized administrative header for the letter
- **generate_update_letter**: Creates the finalized, send-ready text of the contact update notification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **School Contact Update Letter Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a contact update letter for student John Doe (ID: 12345, Grade: 5). Old contact: email: john@old.com. New contact: email: john@new.com. Effective date: 2024-09-01."

**🤖 AI Agent:**
> Dear Parent/Guardian of John Doe (ID: 12345),

Please be advised that the contact information for John Doe has been updated in our records, effective 2024-09-01.

[CHANGED: Email Address]
Old Email: john@old.com
New Email: john@new.com

Sincerely,
School Administration

---

**👤 You:**
> "Check if 'Hand-deliver only' is a valid delivery instruction for the USA region."

**🤖 AI Agent:**
> The requested delivery instruction 'Hand-deliver only' is permitted for the USA region.

---

**👤 You:**
> "What are the differences between these contacts? Old: {phone: '555-1234'}. New: {phone: '555-9876', email: 'test@test.com'}."

**🤖 AI Agent:**
> The following changes were detected: [CHANGED: phone, Added: email]


## ❓ FAQ

**Q: How do I highlight changes in the contact information?**
The `generate_update_letter` tool automatically compares the old and new contact data and explicitly labels any changed fields in the final letter text.

**Q: Can I specify how the letter is delivered?**
Yes, you can provide `deliveryInstructions` to the `generate_update_letter` tool. You can also use `check_delivery_constraints` to verify if your requested method is permitted in a specific region.

**Q: What information is required to generate a letter?**
You need to provide student details (name, ID, grade), the previous contact information, the new contact information, and the effective date of the change.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/school-contact-update-letter-generator](https://vinkius.com/en/ai-agent-connect/school-contact-update-letter-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **School Contact Update Letter Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `school-contact-update-letter-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **School Contact Update Letter Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "school-contact-update-letter-generator": {
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
