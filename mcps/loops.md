# Loops MCP Server

Email marketing and transactional email platform with powerful automation, audience segmentation, and analytics.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/loops)

## Overview
**Category:** marketing-automation
**Tools Count:** 10

## Description
Loops is a modern email marketing and transactional email platform designed for startups and growing businesses. It provides powerful automation for email journeys, audience segmentation, contact management, and detailed analytics. This MCP server enables AI agents to manage contacts, mailing lists, trigger events for automated journeys, send transactional emails, and check suppression statuses — all through natural language commands.

**Key capabilities:**
- Search, create, update, and delete contacts
- Manage mailing lists
- Trigger email journeys with events
- Send transactional emails programmatically
- Check email suppression status
- View sent transactional email history


## Available Tools
- **create_contact**: Requires an email address. Optionally accepts firstName, lastName, and userGroup.

Create a new contact in Loops
- **delete_contact**: This action cannot be undone.

Delete a contact from Loops by ID
- **find_contact**: Returns the contact details if found.

Find a contact in Loops by email address
- **get_contact_suppression**: Suppressed emails will not receive emails. Returns the suppression status for the given email.

Check if an email address is suppressed in Loops
- **list_mailing_lists**: Use this to discover available lists for subscribing contacts.

List all mailing lists in Loops
- **list_transactional_emails**: Optionally accepts a limit parameter to control the number of results returned.

List recently sent transactional emails from Loops
- **send_event**: Requires an eventName. Optionally accepts email and/or userId to identify the recipient.

Send an event to trigger email journeys in Loops
- **send_transactional_email**: Requires the transactionalId. Optionally accepts email and dataVariables (as JSON string) for template variables.

Send a transactional email via Loops
- **test_api_key**: Returns success/failure status.

Test if the Loops API key is valid and working
- **update_contact**: Requires the contact ID. Accepts any fields to update such as firstName, lastName, email, userGroup, etc.

Update an existing contact in Loops by ID


## Installation & Usage

To install and use the **Loops** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loops](https://vinkius.com/mcp/loops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
