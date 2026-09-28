# Local Library Experience Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-library-experience-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Synthesize library requirements, membership status, and program availability into a comprehensive visit plan.

## Description
This MCP server acts as a decision-support engine for library users. It connects AI agents to library services by synthesizing user requirements, membership status, and program availability. Use `plan_library_visit` to generate a complete strategy including enrollment actions and accessibility preparations. You can also use `check_service_eligibility` to verify access rights, `calculate_capacity_availability` to check for open slots, and `resolve_accessibility_requirements` to prepare for specific needs.


## Available Tools (4)
- **calculate_capacity_availability**: Determines if there is enough space or availability for the user and their companions
- **check_service_eligibility**: Validates if a specific user can access a specific library service or program
- **plan_library_visit**: Generates a comprehensive visit strategy based on user needs and library constraints
- **resolve_accessibility_requirements**: Maps user accessibility needs to specific preparation instructions and service modifications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Library Experience Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am an Active member and I want to visit the library on October 12th for a coding workshop and a book lending session. I will be accompanied by one child. Can you plan my visit?"

**🤖 AI Agent:**
> Your visit plan for October 12th includes the coding workshop and book lending. Enrollment actions: Register for the workshop via the portal. Visit preparation: Bring your library card and a valid ID. Participation roles: You are the Primary Attendee and your child is the Observer.

---

**👤 You:**
> "I have wheelchair accessibility needs. Can I book a study room for tomorrow?"

**🤖 AI Agent:**
> Yes, the study room is accessible. Required preparations: Ensure you notify the front desk upon arrival. Service modifications: The library will ensure the path to the room is clear of obstructions.

---

**👤 You:**
> "Am I eligible to use the digital resources if my membership is Suspended?"

**🤖 AI Agent:**
> No, your current membership status as Suspended prevents access to digital resources and other library services.


## ❓ FAQ

**Q: How can I check if I am allowed to join a specific workshop?**
You can use the `check_service_eligibility` tool to verify if your current membership status permits access to specific service types like workshops or room bookings.

**Q: Can this tool help me prepare for accessibility needs?**
Yes, the `resolve_accessibility_requirements` tool maps specific needs like wheelchair access or braille to required preparations and service modifications.

**Q: How do I know if a study room is available for my group?**
Use the `calculate_capacity_availability` tool with the specific service ID and the total number of participants to see if there are remaining slots.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-library-experience-plan](https://vinkius.com/en/ai-agent-connect/local-library-experience-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Library Experience Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-library-experience-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Library Experience Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-library-experience-plan": {
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
