# Lob MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lob)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate physical mail, postcards, checks, and address verification through Lob's print and mail API.

## Description
Lob MCP Server enables AI agents to send physical mail directly from your applications. Create and mail letters, postcards, and checks programmatically through Lob's print and mail API. Verify US and international addresses, autocomplete partial addresses, and manage your address book. Build reusable HTML templates for personalized mailings. Perfect for automating vendor payments, customer communications, marketing campaigns, payroll checks, and direct mail operations. All mail is printed, processed, and delivered within 24 hours via USPS integration.


## Available Tools
- **autocomplete_us_address**: Autocomplete a partial US address
- **cancel_letter**: Only works if status is still "processing".

Cancel a letter before it enters production
- **create_address**: Requires name and address_line1.

Create a new address in your Lob address book
- **create_bank_account**: Requires description, routing_number, account_number, account_type (company/individual), and signatory.

Add a bank account for sending checks
- **create_check**: Requires recipient (to), bank account ID, and amount. Optional: memo, logo, description.

Create and mail a physical check through Lob
- **create_letter**: Requires recipient (to), sender (from), and file content. Supports HTML templates with merge variables, color options, and mail type selection.

Create and mail a physical letter through Lob
- **create_postcard**: Requires recipient (to) and front design. Optional: back design, message, merge variables.

Create and mail a physical postcard through Lob
- **create_template**: Create a reusable HTML template for mailings
- **delete_address**: Delete an address from your Lob address book
- **get_address**: Get details of a specific address
- **get_check**: Get details of a specific check by ID
- **get_letter**: Get details of a specific letter by ID
- **get_postcard**: Get details of a specific postcard by ID
- **get_template**: Get details of a specific template
- **list_addresses**: Use optional limit to control result count.

List addresses in your Lob address book
- **list_bank_accounts**: Use optional limit to control result count.

List bank accounts in your Lob account
- **list_checks**: Track payments, audit disbursements.

List physical checks sent through Lob
- **list_letters**: Each letter includes status, tracking number, and expected delivery date. Use optional limit to control result count.

List physical letters sent through Lob. Track mailings, check delivery status, and review letter history
- **list_postcards**: Use optional limit to control result count.

List physical postcards sent through Lob
- **list_templates**: List HTML templates for mailings
- **verify_us_address**: Verify and standardize a US address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lob** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a letter to John Doe at 123 Main St, New York, NY 10001 with our welcome package HTML template"

**🤖 AI Agent:**
> I'll create a letter using your welcome package template and send it to the specified address. First, I'll create the recipient address, then create the letter with merge variables for personalization.

---

**👤 You:**
> "Verify if this address is deliverable: 185 Berry St, San Francisco, CA 94107"

**🤖 AI Agent:**
> I'll verify the US address to confirm deliverability and standardize the format. This will also add the missing ZIP+4 code and correct any formatting issues.

---

**👤 You:**
> "Send a $500 check to ABC Consulting for consulting services rendered in March"

**🤖 AI Agent:**
> I'll create a physical check for $500 payable to ABC Consulting. This requires a verified bank account in your Lob account. The check will be printed and mailed within 24 hours via USPS.


## ❓ FAQ

**Q: What types of physical mail can I send with Lob?**
Lob supports three main mail types: Letters (formal correspondence, invoices, notifications with customizable color, double-sided printing), Postcards (marketing campaigns, invitations, reminders in 4x6, 6x9, or 6x11 sizes), and Checks (vendor payments, payroll, refunds, rebates with customizable memo lines and company logos). All mail is printed and mailed within 24 hours via USPS.

**Q: How does Lob address verification work?**
Lob's address verification validates and standardizes addresses using USPS data. It corrects formatting, adds missing ZIP+4 codes, fixes typos, and confirms deliverability. The service returns a deliverability status: 'deliverable' (valid and deliverable), 'undeliverable' (cannot be delivered), or 'deliverable_unnecessary' (valid but additional info not needed). This reduces returned mail by up to 5% and ensures your mailings reach the correct destination.

**Q: Can I use HTML templates for personalized mailings?**
Yes! Lob supports HTML templates with merge variables using the Handlebars templating engine. Create a template with placeholders like {{name}}, {{order_number}}, {{delivery_date}}, then pass actual values when creating letters or postcards. This enables personalized, scalable direct mail campaigns. Templates are reusable and can be referenced by ID when creating mailings. You can also embed CSS styling for professional-looking mail designs.

**Q: How long does it take for mail to be delivered?**
Lob prints and mails all items within 24 hours of creation. Delivery time depends on the mail type selected: USPS First Class Mail typically delivers in 2-5 business days, while USPS Standard Mail takes 3-7 business days. You receive a tracking number for each piece of mail to monitor delivery status. Lob also provides expected delivery dates in API responses for planning purposes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lob](https://vinkius.com/mcp/lob)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lob** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lob` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lob** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lob": {
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
