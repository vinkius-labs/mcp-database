# Thoughtly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thoughtly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/thoughtly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/thoughtly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication](../categories/communication.md)

Deploy AI voice agents to make or receive calls, manage CRM contacts, and access call histories instantly.

## Description
Connect your **Thoughtly** voice AI platform to any text-based AI agent to seamlessly bridge the gap between text commands and real-world phone calls.

### What you can do

- **Trigger Phone Calls** — Instantly instruct your AI Voice Agents (Interviews) to dial any contact and execute conversational phone workflows
- **Contact Management** — Query your Thoughtly CRM directory, register new leads with phone numbers, and manage their details
- **Call Logs & Transcripts** — Retrieve detailed call histories, metadata, and full transcripts of conversations conducted by your voice agents
- **Agent Fleet Control** — List and inspect all your active AI Voice Agents to deploy the right persona for each outbound campaign

### How it works

1. Subscribe to this server
2. Enter your Thoughtly API Token and Team ID
3. Start commanding your voice agents directly from Claude, Cursor, or any MCP-compatible client

Your text agent becomes the ultimate dispatcher, effortlessly ordering your voice agents to interact with the real world through natural language.

### Who is this for?

- **Sales Development Reps** — automate outbound qualification campaigns by triggering voice agents for new leads instantly
- **Customer Support Teams** — quickly query the transcript of past AI interactions without opening a dashboard
- **Operations Managers** — orchestrate complex communication workflows across both text and voice channels simultaneously


## Available Tools
- **create_contact**: Optionally includes first name, last name, email.

Create a new Thoughtly contact
- **delete_contact**: Delete a Thoughtly contact
- **get_call_history**: Get details and transcript for a specific call
- **get_contact**: Get specific Thoughtly contact details
- **get_interview**: Get details for a specific Thoughtly Voice Agent
- **list_calls**: List past phone calls (Call logs)
- **list_contacts**: List Thoughtly contacts
- **list_interviews**: List Thoughtly Voice Agents (Interviews)
- **trigger_call**: Trigger an AI outbound phone call
- **update_contact**: Update an existing Thoughtly contact
- **get_user**: Get Thoughtly user details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Thoughtly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available Voice Agents in Thoughtly."

**🤖 AI Agent:**
> I've fetched your agents. You currently have 'Sales SDR Persona' (ID: INT-881) and 'Support Desk Assistant' (ID: INT-204) ready to make or receive calls.

---

**👤 You:**
> "Create a new contact with the phone number +1234567890 and tell the Sales SDR Voice Agent to call them."

**🤖 AI Agent:**
> Contact successfully created with ID CON-1029. I have just triggered the call using the Sales SDR Voice Agent (INT-881). The system is dialing now.

---

**👤 You:**
> "Get the call transcript for the latest interaction with Call ID CAL-554."

**🤖 AI Agent:**
> Extracting call data... The AI successfully booked an appointment. Here is the transcript: 'AI: Hello, are you available next Tuesday? Human: Yes, 2 PM works. AI: Great, confirmed.'


## Installation & Usage

To install and use the **Thoughtly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thoughtly](https://vinkius.com/mcp/thoughtly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
