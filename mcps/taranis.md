# Taranis MCP Server

Access AI-powered crop scouting via Taranis — detect weeds, diseases, pests, nutrient deficiencies, and get scouting recommendations from ultra-high-resolution imagery.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/taranis)

## Overview
**Category:** the-unthinkable
**Tools Count:** 12

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


## Available Tools
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


## Installation & Usage

To install and use the **Taranis** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/taranis](https://vinkius.com/mcp/taranis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
