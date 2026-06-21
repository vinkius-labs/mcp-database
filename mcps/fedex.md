# FedEx MCP Server

AI logistics: track shipments, get rates, create shipments, and find locations via agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fedex)

## Overview
**Category:** industry-titans
**Tools Count:** 9

## Description
### What you can do

Connect AI agents to the FedEx API suite for end-to-end logistics management:

- **Track packages** in real-time with detailed scan history and delivery estimates
- **Track multiple packages** simultaneously for batch monitoring
- **Get shipping rates** across all FedEx services (Express, Ground, Freight)
- **Create shipments** and generate shipping labels directly
- **Validate addresses** to prevent delivery failures
- **Find nearby FedEx locations** (offices, drop boxes, ship centers)
- **Verify postal codes** and check service availability between locations
- **Get proof of delivery** documents for completed shipments

### How it works

1. **Get your FedEx API credentials** from the FedEx Developer Portal
2. **Ask your AI agent** to track shipments, quote rates, or create shipments
3. **Natural language commands** replace manual FedEx website navigation
4. **Production-ready data** directly from FedEx's operational systems

### Who is this for?

Essential for **e-commerce businesses**, **warehouse managers**, **shipping coordinators**, **customer support teams**, and **logistics professionals**. Let AI agents automate tracking updates, compare shipping costs, validate customer addresses, and find drop-off locations. Perfect for businesses shipping 10+ packages daily who want to eliminate manual tracking, streamline label generation, and reduce delivery exceptions through automated address validation.


## Available Tools
- **check_service_availability**: Includes service names, transit times, and availability status. Use this to verify if Express, Ground, or Freight services operate between specific postal codes before quoting or booking shipments.

Check if FedEx shipping services are available between two locations
- **create_shipment**: Requires shipper/recipient details, package weight/dimensions, and service type. Returns tracking number, label format, and estimated delivery date. Use this to generate labels for outbound shipments or process returns.

Create a FedEx shipment and generate a shipping label
- **find_locations**: Includes location type (FedEx Office, Ship Center, Drop Box), address, hours of operation, and services offered. Use this to find where to drop off packages, print labels, or access packing supplies.

Find nearby FedEx locations (drop-off points, offices, or drop boxes)
- **get_postal_code**: Use this to verify postal codes before shipping or to resolve ambiguous addresses.

Validate a postal/ZIP code and get location details
- **get_proof_of_delivery**: Returns POD image URL, delivery date, recipient name, and signature status. Use this to confirm successful delivery for billing disputes, insurance claims, or customer inquiries.

Get proof of delivery (POD) document for a delivered FedEx package
- **get_rates**: Requires origin/destination postal codes, package weight, and dimensions. Returns service type, rate, currency, and estimated delivery date. Use this to compare shipping costs or choose the most economical service.

Get shipping rates and transit times for FedEx services
- **track_multiple_packages**: Returns an array of results with status, scans, and delivery info for each. Requires an array of tracking numbers. Use this for batch monitoring of multiple shipments or checking the status of a multi-piece delivery.

Track multiple FedEx packages in a single request
- **track_package**: Requires the 12-15 digit tracking number. Use this to monitor shipment progress, verify delivery, or investigate delays.

Track a single FedEx package by tracking number
- **validate_address**: Returns standardized format, validation status, and suggestions if the address is incorrect. Requires street lines, city, state, and postal code. Use this to prevent delivery failures, correct typos in addresses, or verify international addresses before shipping.

Validate and standardize a shipping address with FedEx


## Installation & Usage

To install and use the **FedEx** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fedex](https://vinkius.com/mcp/fedex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
