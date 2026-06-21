# Vertiv Environet MCP Server

Monitor data center environmental sensors, alerts, and thresholds via Vertiv Environet Alert API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vertiv-environet)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Vertiv Environet** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vertiv-environet](https://vinkius.com/mcp/vertiv-environet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
