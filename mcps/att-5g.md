# AT&T 5G MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/att-5g)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/att-5g-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/att-5g-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access Open Gateway 5G Network APIs -- Number Verify, Device Location, SIM Swap detection, Quality on Demand, and Network Slicing via AT&T.

## Description
Connect your **AT&T 5G** account to any AI agent and unlock the full power of Open Gateway / CAMARA-compliant network APIs through natural conversation.

### What you can do

- **Number Verify** -- Silently confirm a user's phone number matches their current device without SMS OTP friction
- **Device Location** -- Get approximate geographic positioning via network-based cell tower triangulation (with user consent)
- **SIM Swap Detection** -- Detect recent SIM card changes to prevent account takeovers and fraud before they happen
- **Quality on Demand** -- Request guaranteed network profiles (low latency, high throughput, reliable transmission) for critical sessions
- **Network Slicing** -- Provision, monitor, and decommission dedicated 5G network slices with custom SLA parameters for enterprise use
- **Roaming Status** -- Check if a device is roaming on a foreign network and apply correct billing or routing rules
- **Session Auditing** -- List active and historical QoD sessions to audit premium service consumption

### How it works

1. Subscribe to this server
2. Enter your AT&T 5G API Access Token
3. Start querying network capabilities from Claude, Cursor, or any MCP-compatible client

No more writing custom HTTP clients to hit the AT&T Developer Portal. Your AI agent becomes your 5G network operations console.

### Who is this for?

- **Security Engineers** -- block SIM-swap fraud, verify identities without OTP, and enforce geo-fencing policies
- **Network Architects** -- provision network slices, monitor QoD session health, and audit enterprise SLA compliance
- **Product Teams** -- integrate location-aware features, optimize real-time app performance, and manage roaming billing
- **IoT Operators** -- guarantee connectivity for critical deployments with dedicated slice isolation


## Available Tools
- **check_roaming_status**: Use this to apply correct billing rates, trigger roaming alerts, or optimize routing for international travelers.

Check if a device is currently roaming on a foreign network
- **check_sim_swap**: Returns days since last swap or a boolean indicating recent activity. Use this to block account takeovers attempts, verify identity before password resets, or trigger step-up authentication.

Detect if a SIM card has been swapped recently for fraud prevention
- **create_network_slice**: Requires slice name, SLA profile, and target device group. Returns slice ID and provisioning status. Use this for IoT deployments, private enterprise networks, or guaranteed performance applications.

Provision a new dedicated 5G network slice for an enterprise use case
- **delete_network_slice**: Requires slice ID. Use this to clean up unused slices, reduce costs, or retire temporary deployments.

Decommission and delete an existing 5G network slice
- **get_device_location**: Requires user consent per CAMARA standards. Returns latitude, longitude, and accuracy radius in meters. Use this for geo-fencing, localized content delivery, or emergency services routing. Do not use for precise GPS tracking.

Get approximate geographic location of an AT&T 5G device
- **get_network_slice_info**: Includes SLA parameters, allocated resources, and connected devices. Use this to monitor slice health or verify enterprise SLA compliance.

Get details of a specific 5G network slice
- **list_network_sessions**: Use this to audit network usage, track premium service consumption, or troubleshoot active sessions.

List active and historical network QoD sessions
- **request_quality_on_demand**: Choose profiles like "low_latency" (gaming/VR), "high_throughput" (video), or "reliable_transmission" (IoT). Returns session ID and active duration. Use this to optimize real-time applications, prioritize critical downloads, or enhance remote worker connectivity.

Request guaranteed network quality (low latency/high bandwidth) for a session
- **verify_number**: Eliminates SMS OTP friction. Requires the phone number in E.164 format (e.g., +12125551234). Returns verification status and confidence score. Use this for seamless user onboarding, secure login, or fraud prevention.

Silently verify a user's phone number without SMS OTP


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AT&T 5G** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the phone number +12125551234 had a SIM swap in the last 7 days."

**🤖 AI Agent:**
> I've checked the SIM swap history for +12125551234. No SIM swap events detected in the last 7 days (168 hours). The last recorded swap was 45 days ago. This number appears stable -- safe to proceed with identity verification.

---

**👤 You:**
> "Create a low-latency network slice called 'TradingFloor-Prime' for our enterprise deployment."

**🤖 AI Agent:**
> Network slice 'TradingFloor-Prime' has been successfully provisioned. Slice ID: NS-7a3b9c. SLA profile: low_latency with ultra-reliable parameters. The slice is active and ready to accept device connections. Estimated provisioning time was 12 seconds.

---

**👤 You:**
> "Verify the phone number +14155559876 for user login without sending an SMS code."

**🤖 AI Agent:**
> Number Verify completed successfully for +14155559876. The phone number is confirmed to match the device currently active on the AT&T 5G network. Confidence score: 99.2%. No OTP was sent -- verification was silent and frictionless. User can proceed with login.


## Installation & Usage

To install and use the **AT&T 5G** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/att-5g](https://vinkius.com/mcp/att-5g)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
