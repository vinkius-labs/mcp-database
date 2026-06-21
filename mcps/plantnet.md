# PlantNET MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plantnet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Identify plant species, diseases, and cultivated varieties using the Pl@ntNet AI engine — analyze images and access global taxonomic data.

## Description
Connect the **Pl@ntNet** API to your AI agent to transform it into a powerful botanical assistant. This server allows you to identify thousands of plant species, detect diseases, and explore taxonomic referentials directly through natural conversation.

### What you can do

- **Species Identification** — Submit image URLs of leaves, flowers, fruits, or bark to identify species across global or regional projects.
- **Disease & Pest Detection** — Analyze plant health by identifying common diseases and pests from visual symptoms.
- **Cultivated Varieties** — Specifically identify crops and cultivated plant varieties (varieties/crops) from images.
- **Taxonomic Exploration** — List available projects, browse species lists, and align scientific names with official taxonomies.
- **Advanced Surveys** — Perform multi-species identification on high-resolution imagery (Beta) and estimate processing costs.

### How it works

1. Subscribe to this server
2. Enter your PlantNET API Key
3. Start identifying plants from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Botanists & Researchers** — Quickly verify species names and access regional taxonomic databases.
- **Farmers & Gardeners** — Identify pests and diseases affecting crops to take timely action.
- **Nature Enthusiasts** — Learn about the flora around you by simply providing a photo URL.


## Available Tools
- **list_diseases**: List identifiable plant diseases
- **get_quota**: Check current API quota
- **align_species_name**: Align a species name within a project
- **estimate_survey_cost**: Estimate cost for a multi-species survey
- **get_daily_quota**: Check daily API usage
- **list_languages**: Get the list of supported language codes
- **list_projects**: List Pl@ntNet projects (taxonomic referentials)
- **get_quota_history**: Check API quota history (Contractualized only)
- **get_status**: Check Pl@ntNet API service health status
- **identify_disease**: Identify plant diseases and pests from images
- **identify_species**: Project can be "all" or a specific project ID.

Identify a plant species from images
- **identify_variety**: Identify cultivated plant varieties from images
- **list_species**: Can be scoped to a specific project or global.

List species, optionally filtered by project
- **list_varieties**: List identifiable cultivated plant varieties
- **search_observations**: Search DarwinCore plant observations
- **search_plots**: Search DarwinCore plots
- **survey_tiles**: g., quadrat or drone imagery) to identify multiple species.

Identify multiple species in a single high-resolution image (Beta)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PlantNET** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify this plant species from the image: https://example.com/flower.jpg. It's a flower."

**🤖 AI Agent:**
> I've analyzed the image. With a confidence of 98%, this is identified as *Rosa canina* (Dog Rose). It belongs to the Rosaceae family.

---

**👤 You:**
> "Check if there are any diseases on this leaf: https://example.com/sick-leaf.jpg"

**🤖 AI Agent:**
> The analysis suggests a high probability of *Puccinia graminis* (Wheat stem rust). I recommend checking for reddish-brown spores on the leaf surface.

---

**👤 You:**
> "List the first 10 species available in the 'k-world-flora' project."

**🤖 AI Agent:**
> Fetching species from 'k-world-flora'... Here are the first 10: 1. *Abies alba*, 2. *Abies balsamea*, 3. *Abies concolor*... Would you like to see more details for any of these?


## ❓ FAQ

**Q: How can I identify a plant from a photo URL?**
Use the `identify_species` tool. Provide the image URL and specify the organ shown (e.g., 'flower', 'leaf'). You can set the project to 'all' for a global search.

**Q: Can the AI detect if my plant has a disease?**
Yes! Use the `identify_disease` tool with an image of the affected plant. It will return potential diseases or pests (EPPO codes) identified by the engine.

**Q: How do I find which botanical projects are available for my location?**
Use the `list_projects` tool. You can optionally provide latitude (`lat`) and longitude (`lon`) to filter projects relevant to your specific geographic area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plantnet](https://vinkius.com/mcp/plantnet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PlantNET** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `plantnet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PlantNET** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plantnet": {
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
