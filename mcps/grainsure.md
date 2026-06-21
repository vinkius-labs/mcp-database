# GrainSure MCP Server

Access silo monitoring via GrainSure — track grain fill levels, usage rates, predicted days to empty, and manage deliveries from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/grainsure)

## Overview
**Category:** iot-hardware
**Tools Count:** 12

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


## Available Tools
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


## Installation & Usage

To install and use the **GrainSure** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grainsure](https://vinkius.com/mcp/grainsure)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
