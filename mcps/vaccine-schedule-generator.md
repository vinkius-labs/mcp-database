# Vaccine Schedule Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vaccine-schedule-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Automated vaccination timeline and booster calculator for dogs and cats.

## Description
The Vaccine Schedule Generator provides precise immunization timelines for pets. Using `generate_vaccine_schedule`, you can create a complete chronological list of required vaccinations from birth through adulthood. The `check_vaccine_compliance` tool verifies if a pet's current records meet medical requirements, identifying any missing or overdue doses. Additionally, use `predict_upcoming_boosters` to scan for upcoming vaccination events within a specified timeframe, helping you plan veterinary visits in advance.


## Available Tools (3)
- **check_vaccine_compliance**: Checks if a pet is up to date with vaccinations
- **predict_upcoming_boosters**: Predicts upcoming booster events
- **generate_vaccine_schedule**: Generates a complete vaccination schedule for a pet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vaccine Schedule Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a full vaccination schedule for a dog born on 2023-05-15."

**🤖 AI Agent:**
> The complete schedule for your dog includes: V8/V10 on 2023-06-19, Rabies on 2023-07-17, and Canine Influenza on 2023-08-14.

---

**👤 You:**
> "Is my cat up to date? Born 2024-01-10, administered: [{"vaccineName": "Triple", "date": "2024-02-15"}]"

**🤖 AI Agent:**
> Status: incomplete. Missing vaccines: Rabies, Leukemia.

---

**👤 You:**
> "What vaccinations are due for a cat born on 2023-12-01 in the next 60 days?"

**🤖 AI Agent:**
> Upcoming events: Rabies due on 2024-06-01.


## ❓ FAQ

**Q: How do I generate a full vaccination schedule?**
Use the `generate_vaccine_schedule` tool by providing the pet's species (dog or cat) and their birth date in YYYY-MM-DD format.

**Q: Can I check if my pet is overdue for a vaccine?**
Yes, use the `check_vaccine_compliance` tool. You will need to provide the species, birth date, and a JSON array of vaccines already administered.

**Q: How can I see which vaccines are coming up soon?**
The `predict_upcoming_boosters` tool allows you to specify a window of days to scan for any upcoming vaccination events.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vaccine-schedule-generator](https://vinkius.com/mcp/vaccine-schedule-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vaccine Schedule Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vaccine-schedule-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vaccine Schedule Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vaccine-schedule-generator": {
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
