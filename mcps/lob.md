# Lob MCP Server

Automate physical mail, postcards, checks, and address verification through Lob's print and mail API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/lob)

## Overview
**Category:** customer-support
**Tools Count:** 21

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


## Installation & Usage

To install and use the **Lob** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lob](https://vinkius.com/mcp/lob)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
