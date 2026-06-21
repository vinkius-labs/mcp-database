# Random User Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/random-user-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate high-quality random user data for testing and prototyping — names, emails, and profile photos directly via AI.

## Description
Populate your applications and prototypes with realistic user data instantly. The **Random User Generator** MCP server connects to the RandomUser.me API to provide thousands of unique profiles with specific filters for gender, nationality, and custom fields.

### What you can do

- **Bulk Generation** — Create up to 5,000 user profiles in a single request for stress testing and database seeding
- **Deterministic Data** — Use specific seeds to ensure the same set of users is generated every time, perfect for consistent UI testing
- **Localized Profiles** — Filter by nationality (e.g., US, GB, FR, BR) to match your application's target demographic
- **Custom Payloads** — Include or exclude specific fields like login credentials, location, or contact info to keep your data lean
- **Pagination Support** — Navigate through large sets of generated data using page numbers combined with seeds

### How it works

1. Subscribe to this server
2. No API key is required for the public service
3. Start generating mock data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Frontend Developers** — quickly fill UI components with realistic names and avatars without manual entry
- **QA Engineers** — generate large datasets for performance testing and edge-case validation
- **Product Designers** — create high-fidelity mockups with diverse and realistic user profiles


## Available Tools
- **generate_users**: Supports filtering by gender, nationality, and pagination via seed.

Generate random user data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Random User Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate 5 random female users from Germany and the UK."

**🤖 AI Agent:**
> I've generated 5 female profiles from DE and GB. Each includes full names, emails, and profile pictures. Would you like to see the specific location details for these users?

---

**👤 You:**
> "Create 10 random users but only include their name, email, and nationality."

**🤖 AI Agent:**
> I've fetched 10 user profiles filtered to show only names, emails, and nationalities as requested. This keeps the data payload clean for your prototype.

---

**👤 You:**
> "Generate a random user using the seed 'vurb-testing' for deterministic results."

**🤖 AI Agent:**
> Using the seed 'vurb-testing', I've generated a profile for 'Jennie Nichols'. You can use this same seed anytime to retrieve this exact user data again.


## ❓ FAQ

**Q: Can I generate users from specific countries like the US or France?**
Yes! Use the `generate_users` tool and provide a comma-separated list of nationalities in the `nat` parameter (e.g., 'US,FR').

**Q: How do I ensure I get the same random users every time I run a test?**
You can use the `seed` parameter in the `generate_users` tool. Providing the same string as a seed will return the exact same set of user data for deterministic testing.

**Q: Is it possible to exclude sensitive fields like login passwords from the response?**
Absolutely. Use the `exc` parameter to list fields you want to exclude (e.g., 'login'), or use `inc` to specify only the fields you need (e.g., 'name,email,picture').


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/random-user-generator](https://vinkius.com/mcp/random-user-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Random User Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `random-user-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Random User Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "random-user-generator": {
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
