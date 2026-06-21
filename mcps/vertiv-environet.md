# Vertiv Environet MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vertiv-environet)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vertiv-environet-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vertiv-environet-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Monitor data center environmental sensors, alerts, and thresholds via Vertiv Environet Alert API.

## Description
Connect **Vertiv Environet Alert** to any AI agent and gain real-time visibility into your critical infrastructure's environmental health — temperature, humidity, water leaks, smoke, and active alarms.

### What you can do
- **Site Management** — List all monitored facilities and data centers
- **Sensor Monitoring** — Retrieve real-time readings from temperature, humidity, and airflow sensors
- **Active Alerts** — View and filter active alarms by severity (Critical, Major, Minor)
- **Alert Acknowledgement** — Acknowledge alerts to track operator response and maintain audit trails
- **Threshold Management** — View and update high/low limits for environmental sensors
- **Alert History** — Analyze historical alarm data for root cause analysis and SLA reporting
- **System Health** — Verify the monitoring platform's operational status
- **Audit Logs** — Review user activity and configuration changes for compliance

### How it works
1. Subscribe to this server
2. Enter your Vertiv Environet API Key and Base URL
3. Start monitoring your data center environment from Claude, Cursor, or any MCP-compatible client

Vertiv Environet provides real-time infrastructure optimization, ensuring your critical IT environments remain within safe operating parameters.

### Who is this for?
- **Data Center Operators** — instantly check rack temperatures, acknowledge critical humidity alarms, and review historical trends
- **Facility Managers** — monitor site-wide environmental health and ensure compliance with ASHRAE thermal guidelines
- **NOC Teams** — integrate environmental alerts into centralized monitoring dashboards via AI agent automation


## Available Tools
- **acknowledge_alert**: Requires the alertId and the userId of the operator acknowledging it. Acknowledged alerts are removed from the "active" list and moved to history. Essential for audit trails and shift handovers.

Acknowledge an active alarm to indicate it is being investigated
- **get_alert_history**: Optional siteId and limit parameters. Use this for root cause analysis, SLA reporting, or identifying recurring environmental issues.

View historical alarm records for analysis and reporting
- **get_active_alerts**: Can filter by severity (Critical, Major, Minor, Warning) or by site. Critical alerts often indicate immediate risk to equipment or operations. Use this to prioritize operational response.

Get currently active environmental alarms and warnings
- **get_sensor_reading**: Use this for precise monitoring of critical assets (e.g., specific server rack temperature or UPS room humidity).

Get the current real-time reading from a specific sensor
- **get_sensors**: Optional siteId filters results to a specific facility. Use this to discover available monitoring points.

List environmental sensors deployed across monitored sites
- **get_sites**: Use this to identify which site IDs to use for further filtering of sensors and alerts.

List all monitored sites and facilities in the Environet system
- **get_system_health**: Use this to verify if the monitoring platform is online and functioning correctly before trusting sensor data.

Check the operational status of the Environet monitoring system itself
- **get_thresholds**: Optional sensorId filters to a specific sensor. Use this to audit current safety limits and ensure they match operational requirements.

View configured alarm thresholds for sensors
- **update_threshold**: Changes trigger new alarms if readings cross the new boundaries. Use this to adjust sensitivity based on seasonal changes or equipment updates.

Modify alarm thresholds for a sensor
- **get_user_activity**: Use this for security auditing and operational compliance.

View audit log of user actions within the Environet system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vertiv Environet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all critical environmental alerts right now."

**🤖 AI Agent:**
> Found 2 Critical alerts: 1) Rack A4 Temp High — 32°C (Threshold: 27°C). 2) UPS Room Humidity Low — 25% (Threshold: 30%). Immediate action recommended.

---

**👤 You:**
> "What's the current temperature in Server Room B?"

**🤖 AI Agent:**
> Current reading for Room B Temp Sensor: 22.4°C (Status: Normal). Last updated 2 mins ago. High limit is 27°C.

---

**👤 You:**
> "Acknowledge alert ID 98765 by operator Admin."

**🤖 AI Agent:**
> Alert 98765 successfully acknowledged by Admin. Status updated to Investigating.


## Installation & Usage

To install and use the **Vertiv Environet** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vertiv-environet](https://vinkius.com/mcp/vertiv-environet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
