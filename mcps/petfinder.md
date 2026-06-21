# Petfinder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/petfinder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Largest adoptable pet database — search dogs, cats, and organizations via AI.

## Description
Transform how you discover adoptable companions with the **Petfinder** MCP server. This integration provides your AI agent with real-time access to hundreds of thousands of pets across North America. Your agent can instantly search for specific breeds, filter by location, and retrieve detailed descriptions and metadata for adoptable animals and welfare organizations. Whether you are looking for a new family member or auditing local shelter capacities, your agent acts as a dedicated adoption counselor through natural conversation.

### What you can do

- **Animal Discovery** — Search for thousands of adoptable pets by type, breed, location, and status.
- **Deep Profile Auditing** — Fetch complete metadata, descriptions, and contact information for individual animals.
- **Organization Lookup** — List and inspect shelters and animal welfare organizations registered with Petfinder.
- **Breed Intelligence** — Retrieve recognized breeds and specific metadata for various animal types.
- **Nearby Search** — Quickly find animals within a specific radius of any ZIP code or city.

### How it works

1. Subscribe to this server
2. Enter your Petfinder API Key and API Secret
3. Start managing your pet discovery from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Prospective Adopters** — instantly find pets that match their specific lifestyle and location requirements.
- **Animal Welfare Researchers** — analyze adoption trends and organization metadata across different regions.
- **Veterinarians & Techs** — quickly retrieve breed information and local shelter data for client education.
- **Community Volunteers** — monitor available animals in their area to help with promotion and matching.


## Available Tools (8)
- **get_animal**: Get details for a specific animal
- **get_organization**: Get organization details
- **get_animal_type**: Get details for an animal type
- **list_animals**: List adoptable animals
- **list_breeds**: List breeds for an animal type
- **list_organizations**: List animal welfare organizations
- **list_animal_types**: g., Dog, Cat, Small & Furry).

List available animal types
- **search_nearby_animals**: Search for animals near a location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Petfinder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find adoptable 'Siberian Husky' dogs in New York."

**🤖 AI Agent:**
> I've searched Petfinder for Siberian Huskies in New York. I found 12 dogs, including 'Luna' and 'Rocky', currently available at local shelters. Would you like to see their details?

---

**👤 You:**
> "Show me animal shelters near ZIP code 90210."

**🤖 AI Agent:**
> Retrieving organizations near Beverly Hills... I've identified 5 active animal welfare groups, including 'LA Animal Services'. I can give you their contact info if you're ready to reach out.

---

**👤 You:**
> "What are the common color patterns for cats?"

**🤖 AI Agent:**
> According to Petfinder's data, common cat color patterns include 'Calico', 'Tabby', 'Tortoiseshell', and 'Point'. I can also list the specific coats recognized for cats if you'd like.


## ❓ FAQ

**Q: Can I search for specific breeds like 'Golden Retriever' near my ZIP code?**
Yes! Use the `list_animals` tool, provide 'Golden Retriever' in the `breed` parameter and your ZIP code in the `location` parameter. Your agent will find all matching dogs in your area.

**Q: How do I get the contact information for a shelter that has a pet I'm interested in?**
Every animal record returned by `get_animal` includes an `organization_id`. Use the `get_organization` tool with that ID to retrieve the shelter's full address, phone number, and email.

**Q: Is there a limit to the search radius?**
Yes, Petfinder supports a search radius up to 500 miles from the provided location. You can specify the distance using the `search_nearby_animals` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/petfinder](https://vinkius.com/mcp/petfinder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Petfinder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `petfinder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Petfinder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "petfinder": {
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
