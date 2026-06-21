# GrainSure MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/grainsure)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Access silo monitoring via GrainSure — track grain fill levels, usage rates, predicted days to empty, and manage deliveries from any AI agent.

## Description
Connect your **GrainSure Silo Monitoring API** to any AI agent and take full control of real-time grain fill level tracking, usage rate analysis, predictive days-to-empty forecasting, and automated delivery management through natural conversation.

### What you can do

- **Silo Management** — List and manage all grain silos with current fill levels, grain types, and monitoring status
- **Real-Time Fill Levels** — Get current grain fill percentage and remaining tonnes for each silo
- **Usage Tracking** — Monitor historical grain consumption rates and identify usage trends
- **Days to Empty** — Get AI-predicted days until each silo runs empty based on current usage patterns
- **Fill Level History** — Track how fill levels have changed over time for delivery effectiveness analysis
- **Low Stock Alerts** — Receive automated alerts when silo levels drop below configured thresholds
- **Delivery Orders** — Create and manage grain delivery orders for timely inventory replenishment
- **Order History** — Track past deliveries, quantities, and supplier performance
- **Sensor Health** — Monitor IoT sensor battery levels, signal strength, and calibration status
- **Farm Overview** — Get comprehensive farm-wide inventory summaries for executive reporting
- **Silo Settings** — Customize alert thresholds, grain types, and usage rate assumptions

### How it works

1. Subscribe to this server
2. Enter your GrainSure API key and base URL (from your platform dashboard)
3. Start monitoring silo levels from Claude, Cursor, or any MCP-compatible client

No more climbing silos to check fill levels or guessing when to order more grain. Your AI acts as a dedicated silo inventory analyst and supply chain assistant.

### Who is this for?

- **Farmers** — monitor grain levels remotely, predict when silos will run empty, and plan deliveries proactively
- **Feed Managers** — track consumption rates, manage multiple silos, and prevent stock-outs
- **Supply Chain Coordinators** — optimize delivery timing, manage suppliers, and reduce emergency orders
- **Agricultural Consultants** — provide data-driven feed management recommendations to clients


## Available Tools (12)
- **create_delivery_order**: Accepts delivery quantity (tonnes), preferred delivery date, supplier information, and any special instructions. Returns order confirmation with order ID, estimated delivery date, and tracking information. Essential for proactive inventory replenishment, automated ordering based on predictions, and supply chain management. AI agents should use this when users ask "order 20 tonnes of wheat for silo 3", "schedule a delivery for silo 5 next week", or need to place delivery orders based on low stock predictions.

Create a new grain delivery order for a specific silo
- **get_current_level**: Returns fill percentage, remaining tonnes, current level height, and last update timestamp. Essential for real-time inventory tracking, delivery planning, and stock management. AI agents should use this when users ask "what is the current fill level in silo 2", "how much grain is left in silo 4", or need immediate stock level data for feed planning and delivery decisions.

Get real-time grain fill level for a specific silo
- **update_silo_settings**: Essential for customizing monitoring behavior, adjusting alert sensitivity, and maintaining accurate silo profiles. AI agents should use this when users ask "change the low stock threshold for silo 3 to 20 percent", "update silo 5 grain type to barley", or need to modify silo monitoring configuration.

Update silo monitoring settings including alert thresholds and grain type
- **get_days_to_empty**: Returns estimated days to empty, predicted empty date, confidence score, and usage rate assumptions. Essential for proactive delivery planning, preventing stock-outs, and optimizing supply chain timing. AI agents should use this when users ask "when will silo 3 run empty", "how many days of feed are left in silo 5", or need predictive supply data for delivery scheduling.

Get AI-predicted days until a silo runs empty based on current usage patterns
- **get_farm_overview**: Essential for executive reporting, farm-wide inventory assessment, and strategic supply planning. AI agents should use this when users ask "give me an overview of all my silos", "what is the total grain inventory across the farm", or need farm-level summaries for management reporting.

Get comprehensive overview of all monitored silos on the farm
- **get_silo_details**: Essential for understanding silo context before analyzing usage data, planning deliveries, or generating inventory reports. AI agents should reference this when users ask "tell me about silo 3", "what grain is stored in silo 5", or need detailed silo metadata for informed decisions.

Get detailed information about a specific grain silo
- **get_silos**: Returns silo IDs, names, locations, grain types, current fill levels, and monitoring status. Essential for farm overview, silo inventory management, and selecting specific silos for detailed analysis. AI agents should use this when users ask "show me all my silos", "list monitored storage units", or need to identify available silos before querying fill levels or usage data.

List all grain silos monitored by GrainSure
- **get_fill_level_history**: Returns time-series fill percentage data with timestamps showing how stock levels have changed over time. Essential for fill trend analysis, delivery effectiveness assessment, and consumption pattern identification. AI agents should use this when users ask "show me fill level trends for silo 1 over the past 60 days", "has silo 2 been filling or depleting", or need historical fill data for inventory management. Optional days parameter controls lookback period.

Get historical fill level readings for a specific silo
- **get_low_stock_alerts**: Returns alert severity (critical, warning, info), affected silo, current fill percentage, threshold level, timestamp, and recommended actions. Essential for proactive inventory management, preventing stock-outs, and timely delivery ordering. AI agents should use this when users ask "show me all low stock alerts", "is silo 3 running low", or need alert data for inventory monitoring. Optional silo_id filters alerts for a specific silo.

Get low stock alerts for silos or a specific silo
- **get_order_history**: Essential for delivery tracking, supplier performance assessment, and inventory replenishment planning. AI agents should reference this when users ask "show me delivery history for silo 2", "when was the last delivery to silo 4", or need order data for supply chain analysis.

Get delivery order history for a specific silo
- **get_sensor_health**: Returns sensor battery level, signal strength, last communication time, calibration status, and operational status (active, low battery, offline, needs calibration). Essential for sensor maintenance, data continuity assurance, and monitoring system reliability. AI agents should reference this when users ask "is the sensor working in silo 5", "does silo 3 need sensor calibration", or need sensor health data for system administration.

Get health status of the level monitoring sensor for a specific silo
- **get_usage_history**: Returns time-series usage data (tonnes per day/week) with timestamps. Essential for consumption trend analysis, feed rate calculation, and delivery timing optimization. AI agents should reference this when users ask "show me grain usage trends for silo 3", "what is the daily consumption rate for silo 5", or need historical usage data for feed planning and inventory forecasting. Optional days parameter controls lookback period.

Get historical grain usage data for a specific silo


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GrainSure** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current fill levels for all my silos."

**🤖 AI Agent:**
> Fetching current silo levels... Silo 1 (Wheat): 78% full, 156 tonnes remaining, sensor updated 2 minutes ago. Silo 2 (Barley): 45% full, 90 tonnes remaining, updated 5 minutes ago. Silo 3 (Corn): 22% full, 44 tonnes remaining — LOW STOCK alert triggered, updated 1 minute ago. Silo 4 (Oats): 91% full, 182 tonnes remaining, updated 3 minutes ago. Total farm inventory: 472 tonnes across 4 silos. Priority action: Silo 3 is approaching critical levels — consider ordering delivery within the next 3-5 days. Would you like predicted days-to-empty for each silo?

---

**👤 You:**
> "How many days until my wheat silo runs empty?"

**🤖 AI Agent:**
> Checking days-to-empty prediction for wheat silo (Silo 1)... Current fill: 78% (156 tonnes). Average daily usage: 3.2 tonnes/day. Predicted days to empty: 49 days. Predicted empty date: May 26, 2026. Confidence: 92%. Usage trend: Stable consumption over the past 30 days with slight increase during the last week. Recommendation: No immediate action required. Consider scheduling next delivery in approximately 35 days to maintain comfortable stock levels. Would you like to see the detailed usage history for this silo?

---

**👤 You:**
> "Order 30 tonnes of barley for silo 2 with delivery next week."

**🤖 AI Agent:**
> Creating delivery order for Silo 2 (Barley)... Order confirmed! Order ID: ORD-2026-0417. Quantity: 30 tonnes of Barley. Preferred delivery date: April 21, 2026. Estimated supplier response time: 24 hours. Current silo status: 45% full (90 tonnes), predicted to last 28 days. This delivery will bring the silo to approximately 90% capacity. You will receive confirmation from the supplier within 24 hours. Would you like to set up an automatic reorder threshold for this silo?


## ❓ FAQ

**Q: Can my AI predict when my silo will run empty based on current usage?**
Yes! Use the `get_days_to_empty` tool with your silo ID. GrainSure AI analyzes current fill levels and historical usage patterns to predict exactly how many days until the silo runs empty, with a confidence score. For deeper analysis, combine with `get_usage_history` to see the consumption trends that drive the prediction. This gives you proactive warning to schedule deliveries before running out.

**Q: How do I set up low stock alerts for my silos?**
Use the `update_silo_settings` tool to configure your low stock threshold percentage (e.g., 20% means alert when silo drops below 20% full). Then use `get_low_stock_alerts` to check for any active alerts. GrainSure will automatically monitor fill levels and trigger alerts when thresholds are breached, giving you timely warning to plan deliveries.

**Q: Can I create a delivery order directly through the API?**
Yes! Use the `create_delivery_order` tool with the silo ID, quantity in tonnes, and optionally a preferred delivery date and supplier. The API will confirm your order with an order ID and estimated delivery date. You can also use `get_days_to_empty` predictions to automatically trigger orders when silos reach critical levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grainsure](https://vinkius.com/mcp/grainsure)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GrainSure** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grainsure` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GrainSure** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grainsure": {
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
