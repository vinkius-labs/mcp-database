# vCard Contacts Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vcard-contacts-parser-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Instantly convert massive iPhone and Android `.vcf` contact exports into structured JSON. Turn your AI into a hyper-intelligent local address book.

## Description
When you export your phone's address book, you get a massive `.vcf` file containing hundreds of contacts formatted in the legacy `BEGIN:VCARD` structure, often bloated with base64-encoded profile pictures. If you ask an LLM to read this raw file, it will exhaust its context window and hallucinate phone numbers and emails.

This MCP is a dedicated contact intelligence engine. It runs 100% local on your machine, instantly stripping away the binary noise and converting the raw vCard format into a beautiful, easily queryable JSON array. The AI sees exactly what it needs: First Name, Last Name, Organization, Phone, and Email.

### The Superpowers

- **100% Air-Gapped Privacy:** Your personal phonebook never leaves your local machine.
- **Zero Hallucination:** Perfect extraction of country codes, emails, and company roles.
- **Massive File Support:** Can instantly process a VCF file containing 5,000+ contacts.
- **Assistant Ready:** Ask your AI: 'Find the phone number for the CTO of Vinkius in my contacts.'


## Available Tools
- **parse_vcard_contacts**: Provide the absolute file path.

Parse a .vcf (vCard) contact export file into structured JSON. Extracts names, phones, emails, and organization details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **vCard Contacts Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my contacts.vcf and give me a list of everyone who works at 'Vinkius'."

**🤖 AI Agent:**
> I found 3 contacts working at Vinkius: John Silva (DevOps), Sarah Connor (Design), and Mike Ross (Legal).

---

**👤 You:**
> "Extract all the email addresses from this vCard export and format them as a CSV."

**🤖 AI Agent:**
> Name,Email
Alice Smith,alice@example.com
Bob Jones,bob@example.org

---

**👤 You:**
> "Look through my contacts and find the phone number for 'Plumber'."

**🤖 AI Agent:**
> The phone number saved under 'Plumber' is +1 (555) 019-8372.


## ❓ FAQ

**Q: Is my address book uploaded to the cloud?**
Never. The vCard parsing is executed completely local on your device. Only the extracted text representation is provided to the AI context.

**Q: Does it support multiple contacts in a single file?**
Yes! It perfectly parses multi-vCard files exported from iOS, Google Contacts, or Android devices, handling thousands of entries seamlessly.

**Q: What happens to the contact profile pictures?**
Profile pictures (PHOTO;ENCODING=b) are intentionally ignored and stripped during parsing to preserve AI context tokens and prevent crashes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vcard-contacts-parser-extended](https://vinkius.com/mcp/vcard-contacts-parser-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **vCard Contacts Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vcard-contacts-parser-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **vCard Contacts Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vcard-contacts-parser-extended": {
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
