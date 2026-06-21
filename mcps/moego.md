# MoeGo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moego)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage your pet care business via MoeGo — track appointments, pets, and customers directly from your AI agent.

## Description
Connect your **MoeGo** pet care business account to your AI agent and streamline your grooming and boarding operations through natural conversation.

### What you can do

- **Appointment Management** — List all scheduled appointments and get detailed status updates.
- **Pet & Customer Profiles** — View registered pets, their owners, and specific care details including breeds and ages.
- **Service & Staff Oversight** — Access your catalog of grooming services and list of active staff members.
- **Scheduling** — Create new service appointments for pets and customers with simple commands.
- **Reputation Monitoring** — Retrieve recent customer reviews and feedback directly within your chat.
- **Business Configuration** — Access general metadata and settings for your MoeGo account.
- **Deep Inspection** — Fetch complete metadata for specific appointments or pets using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your MoeGo API Key
3. Start managing your pet business from Claude, Cursor, or any MCP client

### Who is this for?

- **Pet Groomers & Boarders** — quickly check the day's schedule or look up a pet's details without opening the MoeGo app.
- **Business Owners** — monitor operations, staff, and client growth directly from your communication tools.
- **Receptionists** — verify appointment times and customer info while multitasking.


## Available Tools (10)
- **create_appointment**: Schedule a new appointment
- **get_appointment**: Get appointment details
- **get_business_settings**: Get business configuration
- **get_pet**: Get specific pet details
- **list_appointments**: List grooming appointments
- **list_customers**: List MoeGo customers
- **list_pets**: ) associated with your business.

List all registered pets
- **list_reviews**: List customer reviews
- **list_services**: List grooming services
- **list_staff**: List business staff


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MoeGo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me today's grooming schedule."

**🤖 AI Agent:**
> I've retrieved today's schedule. You have 6 appointments: 'Buddy' (Golden Retriever) at 10:00 AM, 'Luna' (Persian Cat) at 11:30 AM, and 4 more in the afternoon. Would you like the contact details for Buddy's owner?

---

**👤 You:**
> "Get details for the pet with ID pet_123."

**🤖 AI Agent:**
> Inspecting pet_123... This is 'Max', a 3-year-old Beagle. He weighs 12kg and his owner is Sarah Jenkins. Max has a note: 'Sensitive skin, use hypoallergenic shampoo'. Shall I check his last appointment date?

---

**👤 You:**
> "List all our available grooming services and prices."

**🤖 AI Agent:**
> I've fetched your service catalog. You offer 12 services, including 'Full Grooming - Large Dog' ($85.00), 'Puppy's First Bath' ($45.00), and 'Nail Trim' ($15.00). Would you like to check which staff members are assigned to these services?


## ❓ FAQ

**Q: How do I get my MoeGo API Key?**
You can find your API key in the MoeGo dashboard under Settings > Integration. It needs to be the Base64 encoded version as per their documentation.

**Q: Can I see detailed information about a pet's breed?**
Yes! Use the `get_pet` tool with a specific Pet ID. The agent will return the full profile, including breed, age, weight, and any specific care instructions recorded.

**Q: How can I monitor staff performance?**
You can use the `list_staff` tool to see all active professionals and `list_appointments` to track their scheduled workload and completed services.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moego](https://vinkius.com/mcp/moego)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MoeGo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moego` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MoeGo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moego": {
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
