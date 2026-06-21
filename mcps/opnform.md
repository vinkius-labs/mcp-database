# OpnForm MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opnform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/opnform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/opnform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Create beautiful open-source forms with conditional logic, file uploads, and integrations that rival premium form builders.

## Description
Connect your **OpnForm** account to any AI agent and take full control of your form orchestration and data collection through natural conversation. OpnForm is a modern, AI-first, open-source form builder that allows you to create professional forms in seconds.

### What you can do

- **Form & Workspace Orchestration** — List all managed workspaces and forms programmatically to keep your data collection infrastructure always synchronized.
- **Dynamic Form Generation** — Create new forms and update existing fields directly from the AI interface to rapidly deploy surveys or lead magnets.
- **Submission Intelligence** — Retrieve and analyze form responses in real-time via natural language to extract insights without manual exporting.
- **Lifecycle Management** — Delete stale forms and manage workspace metadata using simple AI commands.
- **Account Visibility** — Access your profile and API token capabilities to ensure your automation has the correct permissions.

### How it works

1. Subscribe to this server
2. Enter your OpnForm Personal Access Token from your dashboard settings
3. Start managing your forms and data from Claude, Cursor, or any MCP-compatible client

No more manual dashboard navigation for simple status checks. Your AI acts as a dedicated form operations lead or data coordinator.

### Who is this for?

- **Marketing Teams** — quickly create lead capture forms and monitor submission volume without switching apps.
- **Product Managers** — automate the collection of user feedback and analyze responses via natural conversation.
- **Developers** — integrate real-time form management and data ingestion directly within the chat.


## Available Tools
- **create_form**: Create a new Optform form
- **delete_form**: Delete an Optform form
- **delete_submission**: Delete a form submission
- **get_form**: Get details for a specific Optform form
- **get_submission**: Get details for a specific form submission
- **get_workspace**: Get details for a specific Optform workspace
- **list_forms**: List forms in Optform
- **list_submissions**: List submissions for a form
- **list_workspaces**: List Optform workspaces
- **get_me**: Get current Optform user details
- **update_form**: Update an existing Optform form


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpnForm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active forms in my 'Marketing' workspace."

**🤖 AI Agent:**
> I've retrieved your forms. You have 3 active environments: 'Contact Us', 'Q4 Feedback', and 'Lead Magnet'. Which one would you like to see submissions for?

---

**👤 You:**
> "List all submissions received on my contact form this week with their responses."

**🤖 AI Agent:**
> Your "Contact Us" form (form_821) received 14 submissions this week. 6 are general inquiries, 5 are support requests, and 3 are partnership proposals. The most recent submission is from Elena Torres at Meridian Corp, requesting a product demo for their 200-person engineering team.

---

**👤 You:**
> "Create a new feedback survey form in my Product workspace with rating and comment fields."

**🤖 AI Agent:**
> New form "Product Feedback Survey" created successfully in the Product workspace (ID: form_847). It includes a 5-star rating field, a text area for comments, an email field for follow-ups, and a dropdown for product category selection. The form is currently in draft mode and ready for customization before publishing.


## Installation & Usage

To install and use the **OpnForm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opnform](https://vinkius.com/mcp/opnform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
