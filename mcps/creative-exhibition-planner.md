# Creative Exhibition Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/creative-exhibition-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [art-management](../categories/art-management.md)

Transforms raw exhibition data into cohesive presentation concepts, visitor flows, and operational plans.

## Description
This MCP server acts as a strategic planning engine for curators and artists. It synthesizes artist intent, venue constraints, and confirmed works to generate high-level creative visions via `get_presentation_concept`. It maps physical audience journeys using `plan_visitor_flow`, establishes formal text-review processes with `generate_approval_workflow`, assigns technical responsibilities through `coordinate_installation_roles`, and outlines archival strategies with `create_documentation_plan`.


## Available Tools (5)
- **create_documentation_plan**: Outlines how to record the exhibition for posterity
- **generate_approval_workflow**: Defines the steps required to finalize all textual elements of the exhibition
- **get_presentation_concept**: Generates the high-level creative vision for the exhibition
- **plan_visitor_flow**: Maps out the physical journey of the audience through the space
- **coordinate_installation_roles**: Assigns specific tasks to collaborators based on venue and artist constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creative Exhibition Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a presentation concept for an exhibition of 5 minimalist sculptures in a small, dimly lit gallery."

**🤖 AI Agent:**
> The concept is 'Shadowed Presence', a minimalist journey where the low light emphasizes the silhouettes of the sculptures, creating an intimate and contemplative atmosphere.

---

**👤 You:**
> "Create a visitor flow for a large-scale immersive installation in a warehouse with ramps."

**🤖 AI Agent:**
> The journey follows a circular path, utilizing the ramps to transition between levels, ensuring all visitors can experience the narrative sequence smoothly.

---

**👤 You:**
> "Assign roles for installing heavy bronze works in a space with a 200kg floor limit."

**🤖 AI Agent:**
> Tasks are assigned to specialized handlers and heavy-lifting technicians to ensure the bronze works are placed safely within the floor's weight capacity.


## ❓ FAQ

**Q: How does the tool handle venue constraints?**
The `get_presentation_concept` tool specifically requires venue conditions to ensure the creative vision respects physical limitations like light sensitivity or floor weight limits.

**Q: Can I use this to manage my installation team?**
Yes, by using `coordinate_installation_roles`, you can assign specific tasks to your collaborators based on the technical needs of the works and the venue.

**Q: How is the visitor experience planned?**
The `plan_visitor_flow` tool analyzes the venue layout and accessibility features to create a movement path that aligns with the artist's narrative intent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/creative-exhibition-planner](https://vinkius.com/en/ai-agent-connect/creative-exhibition-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creative Exhibition Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creative-exhibition-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creative Exhibition Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creative-exhibition-planner": {
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
