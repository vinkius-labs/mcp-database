# Harvard Art Museums MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/harvard-art-museums-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Explore the Harvard Art Museums' vast collection — search over 250,000 objects, research artists, and browse exhibitions directly via AI.

## Description
Connect to the **Harvard Art Museums API** and turn your AI agent into a sophisticated art historian. Access one of the world's most comprehensive university art collections through natural conversation.

### What you can do

- **Object Discovery** — Search the entire collection using filters like classification, century, culture, color, or specific years.
- **Artist & People Research** — List and retrieve detailed profiles of artists, donors, and other figures associated with the works.
- **Exhibition Tracking** — Browse past, current, and upcoming exhibitions to stay informed about museum programming.
- **Gallery Exploration** — List physical spaces within the museum building, filtered by floor, to understand where works are displayed.
- **Publication Access** — Query publications that contain images or scholarly information about the museum's artworks.
- **Media Metadata** — Access detailed metadata for images produced by the museums for research and documentation.

### How it works

1. Subscribe to this server
2. Enter your Harvard Art Museums API Key
3. Start exploring art history from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Students** — Quickly find primary sources, object metadata, and artist biographies for academic work.
- **Art Enthusiasts** — Explore the collection by color, culture, or period to discover new favorite pieces.
- **Curators & Educators** — Access exhibition histories and gallery layouts to plan educational content or tours.


## Available Tools
- **get_annotation**: Get specific annotation details
- **get_audio**: Get specific audio details
- **get_exhibition**: Get specific exhibition details
- **get_gallery**: Get specific gallery details
- **get_iiif_gallery_manifest**: Get the IIIF presentation manifest for a gallery
- **get_iiif_object_manifest**: Get the IIIF presentation manifest for an object
- **get_iiif_top_collection**: Get the top level IIIF collection manifest
- **get_image**: Get specific image details
- **get_object**: Get full record for a specific object
- **get_person**: Get specific person details
- **get_publication**: Get specific publication details
- **get_video**: Get specific video details
- **list_activities**: List object-specific activities (pageviews, edits, moves)
- **list_annotations**: List machine-generated and manual annotations on images
- **list_audios**: List audio clips (visual descriptions, etc.)
- **list_centuries**: List centuries used for dating objects
- **list_classifications**: List curatorial categories (Prints, Sculpture, etc.)
- **list_colors**: List CSS3 and extracted color terms
- **list_cultures**: List cultural associations (Dutch, Greek, etc.)
- **list_exhibitions**: List past, current, and upcoming exhibitions
- **list_galleries**: List physical spaces within the museum building
- **list_groups**: List curated groupings (Collection Highlights, etc.)
- **list_images**: List metadata for images produced by the museums
- **list_mediums**: List materials used (Watercolor, Resin, etc.)
- **list_objects**: List objects in the Harvard Art Museums collection
- **list_people**: List people associated with works (artists, donors, etc.)
- **list_periods**: List art movements and time periods
- **list_places**: List geographic locations
- **list_publications**: List publications containing images or info about artworks
- **list_sites**: List physical museum sites and facilities
- **list_spectrums**: List colors in the museum branding spectrum
- **list_supports**: List surfaces used (Wood, Slate, etc.)
- **list_techniques**: List production processes (Red-figure, Etching, etc.)
- **list_videos**: List videos produced by or associated with the museums
- **list_worktypes**: List specific object types (fragment, vessel, etc.)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harvard Art Museums** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 19th-century French paintings in the Harvard Art Museums collection."

**🤖 AI Agent:**
> I've found several 19th-century French paintings. Notable works include 'The Rehearsal' by Edgar Degas (ID: 299842) and 'The Gare Saint-Lazare' by Claude Monet. Would you like the full details for any of these?

---

**👤 You:**
> "List all current exhibitions and their venues."

**🤖 AI Agent:**
> There are currently 4 active exhibitions. Highlights include 'Objects of Addiction' at the Arthur M. Sackler Museum and 'American Watercolors' at the Fogg Museum. Which one would you like to explore further?

---

**👤 You:**
> "Get the full record for object ID 303935."

**🤖 AI Agent:**
> Fetching record 303935... This is 'Self-Portrait' by Vincent van Gogh, oil on canvas, dated 1887. It is currently located in Gallery 2400. It features a vibrant palette of blues and yellows with characteristic brushwork.


## ❓ FAQ

**Q: How can I find artworks from a specific culture or time period?**
You can use the `list_objects` tool and apply filters like `culture` (e.g., 'Japanese') or `century` (e.g., '19th century'). You can also use `yearmade` for more precise dating.

**Q: Is it possible to see which exhibitions are currently running at the museum?**
Yes! Use the `list_exhibitions` tool with the `status` parameter set to 'current'. This will return a list of all active shows with their details.

**Q: Can I search for artworks based on their location within the museum building?**
Absolutely. You can use `list_galleries` to find specific room IDs or floors, and then use the `gallery` filter in `list_objects` to see what is displayed in that specific space.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/harvard-art-museums-alternative](https://vinkius.com/mcp/harvard-art-museums-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Harvard Art Museums** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `harvard-art-museums-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Harvard Art Museums** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "harvard-art-museums-alternative": {
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
