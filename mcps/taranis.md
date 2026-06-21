# Taranis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/taranis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access AI-powered crop scouting via Taranis — detect weeds, diseases, pests, nutrient deficiencies, and get scouting recommendations from ultra-high-resolution imagery.

## Description
Connect your **Taranis AI Scouting API** to any AI agent and take full control of AI-powered crop threat detection, ultra-high-resolution imagery analysis, field scouting recommendations, and precision agriculture decision-making through natural conversation.

### What you can do

- **Organizations** — List all agricultural organizations and farms in your Taranis account
- **Field Management** — View all monitored fields with crop types, boundaries, and growth stages
- **Flight History** — Review all drone and aircraft flight missions with imagery acquisition dates
- **Flight Imagery** — Access ultra-high-resolution orthomosaics, DSMs, and NDVI maps from each flight
- **All Detections** — Get comprehensive AI-detected threats (weeds, diseases, pests, nutrients) in any field
- **Threat Summary** — View consolidated threat severity assessments and trend analysis per field
- **Scouting Recommendations** — Receive AI-powered action plans for targeted field scouting missions
- **Multispectral Analysis** — Access NDVI, NDRE, and GNDVI vegetation indices for vigor assessment
- **Weed Detection** — Identify specific weed species with coverage estimates and herbicide recommendations
- **Disease Detection** — Detect crop diseases with severity levels and fungicide treatment suggestions
- **Nutrient Analysis** — Identify nutrient deficiencies with variable rate fertilization recommendations

### How it works

1. Subscribe to this server
2. Enter your Taranis API token (from the dashboard API settings)
3. Start analyzing crop threats from Claude, Cursor, or any MCP-compatible client

No more manual field scouting or delayed threat identification. Your AI acts as a dedicated precision agriculture analyst and crop health monitoring assistant.

### Who is this for?

- **Farm Managers** — detect crop threats early, prioritize scouting, and optimize treatment timing
- **Agronomists** — analyze ultra-high-resolution imagery, identify weed species, and track disease progression
- **Crop Consultants** — generate scouting recommendations, create treatment plans, and advise clients with data-driven insights
- **Ag Retailers** — identify treatment opportunities, plan product applications, and demonstrate ROI with before/after imagery


## Available Tools (12)
- **get_fields**: Returns field names, IDs, boundaries (GeoJSON polygons), area in hectares/acres, crop type, planting dates, and monitoring status. Essential for farm management overview and selecting target fields for threat detection.

List all agricultural fields monitored by Taranis for a farm
- **get_clients**: Returns client names, IDs, and associated farm counts. Use this after get_organizations to navigate the hierarchy: Organizations → Clients → Farms → Fields.

List clients within a specific Taranis organization
- **get_detections**: Returns detection locations (GPS coordinates), threat types, severity levels, confidence scores, and recommended actions.

Get all AI-detected crop threats (weeds, diseases, pests, nutrient deficiencies) in a field
- **get_disease_detections**: Returns disease locations, pathogen identification, severity levels, and recommended fungicide treatments.

Get crop disease detections and severity assessments for a field
- **get_farms**: Returns farm names, IDs, locations, and field counts. Use this after get_clients to navigate to specific farms before querying fields.

List farms belonging to a specific client
- **get_field_details**: Get detailed information about a specific agricultural field
- **get_map_layers**: Returns layer metadata and download URLs. Essential for crop vigor assessment, variable rate application planning, and growth stage monitoring.

Get map layers (NDVI, imagery, multispectral) for a specific field
- **get_nutrient_detections**: Returns deficiency locations, severity estimates, and variable rate fertilization recommendations.

Get nutrient deficiency detections and fertilization recommendations for a field
- **get_organizations**: Returns organization names, IDs, contact information, and field counts. Essential for multi-account management, selecting target organizations for field analysis, and understanding the scope of monitored agricultural operations.

List all organizations available to the user in Taranis platform
- **get_scouting_recommendations**: Returns specific action items including verification locations, scouting patterns, and treatment suggestions.

Get AI-powered scouting recommendations and action plans for a field
- **get_threats**: Returns threat categories, overall severity ratings, affected area percentages, and priority rankings.

Get consolidated threat summary and severity assessment for a field
- **get_weed_detections**: Returns weed locations, estimated coverage area, species classification, and herbicide resistance indicators.

Get specific weed species detections and infestation maps for a field


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Taranis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all AI-detected threats in my corn field from the latest flight."

**🤖 AI Agent:**
> Analyzing latest flight detections for corn field (field ID: CF-2847)... Found 23 detections across 4 threat categories. WEEDS: 12 patches detected — Waterhemp (7 patches, 2.3% coverage), Palmer Amaranth (3 patches, 1.1%), Giant Ragweed (2 patches, 0.8%). DISEASES: 6 detections — Gray Leaf Spot (moderate severity, 4 locations), Northern Corn Leaf Blight (early stage, 2 locations). PESTS: 3 detections — Corn Rootworm adults (2 locations), European Corn Borer damage (1 location). NUTRIENTS: 2 nitrogen deficiency zones (1.5% combined area). Overall field health: Good with localized treatment needed. Top priority: Waterhemp patches in northeast quadrant. Would you like scouting recommendations for these detections?

---

**👤 You:**
> "Generate scouting recommendations for my soybean field this week."

**🤖 AI Agent:**
> Generating AI scouting recommendations for soybean field (field ID: SB-1923)... Priority 1 (HIGH): Verify Sudden Death Syndrome symptoms in southeast corner — 4 disease detections with moderate severity. Walk pattern: Entry at gate 3, follow east boundary south, check 4 GPS-marked locations. Priority 2 (MEDIUM): Scout for soybean aphids in north-central area — NDVI shows stress patches consistent with early aphid pressure. Priority 3 (LOW): Check nitrogen deficiency zones in western section — 3 small patches identified, consider in-season N application if economic threshold met. Recommended scouting time: 45-60 minutes. Best conditions: Morning hours, dry foliage. Would you like GPS coordinates for each scouting location?

---

**👤 You:**
> "What is the overall threat level and NDVI trend for my wheat field this season?"

**🤖 AI Agent:**
> Analyzing wheat field (field ID: WH-5512)... Current threat level: MODERATE. Season summary: 3 flights completed, 18 total detections. Disease trend: Septoria tritici increasing from 2 to 6 detections over 3 flights — monitor closely. Weed trend: Annual ryegrass stable at 5 patches (1.8% coverage). Nutrient trend: Nitrogen deficiency decreasing after top-dress application — 3 zones down to 1 zone. NDVI trend: Flight 1 (0.45) — tillering stage, Flight 2 (0.68) — stem extension, Flight 3 (0.82) — current heading stage. Field performing above regional average. Recommendation: Continue disease monitoring, no immediate treatment required. Next flight scheduled in 10 days.


## ❓ FAQ

**Q: Can my AI detect specific weed species in my soybean field from Taranis imagery?**
Yes! Use the `get_weed_detections` tool with your field ID to get AI-detected weed infestations with species-level identification. Returns weed locations, estimated coverage area, species classification, growth stage, and herbicide resistance indicators. For a comprehensive view of all threats (weeds, diseases, pests, nutrients), use `get_detections` without a type filter.

**Q: How do I get scouting recommendations based on the latest flight imagery?**
Use the `get_scouting_recommendations` tool with your field ID. Taranis AI analyzes the latest imagery, detected threats, crop growth stage, and field history to generate specific action items including ground truth verification locations, recommended scouting patterns, treatment suggestions, and priority levels. You can also use `get_threats` first to see the overall threat severity before reviewing recommendations.

**Q: What resolution imagery does Taranis capture and how often are flights conducted?**
Taranis captures ultra-high-resolution imagery at sub-millimeter to centimeter level resolution using specialized drone and fixed-wing aircraft. Flight frequency depends on your monitoring plan and crop growth stage — typically every 7-14 days during critical growth periods. Use `get_flights` to see all flight history for a field, and `get_flight_imagery` to access specific imagery products (orthomosaics, DSM, NDVI maps) from any flight mission.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/taranis](https://vinkius.com/mcp/taranis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Taranis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `taranis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Taranis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "taranis": {
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
