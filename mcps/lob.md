# Lob MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lob)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lob-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lob-mcp)
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


## Installation & Usage

To install and use the **Lob** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lob](https://vinkius.com/mcp/lob)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
