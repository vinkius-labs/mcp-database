# Correios do Brazil MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/correios-do-brazil)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/correios-do-brazil-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/correios-do-brazil-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Calculate shipping costs, estimate delivery times, and consult address information via the official Correios REST API.

## Description
Connect your **Correios** account to any AI agent to automate logistics and shipping calculations directly within your workflow.

### What you can do

- **Shipping Calculation** — Calculate precise shipping costs based on origin, destination, weight, and package dimensions for services like SEDEX and PAC.
- **Delivery Estimates** — Get the estimated number of working days for any delivery across Brazil.
- **Address Lookup (CEP)** — Instantly retrieve full address details (street, neighborhood, city, state) from any Brazilian ZIP code.
- **Service Comparison** — Compare different postal service codes to find the best shipping option for your needs.

### How it works

1. Subscribe to this server
2. Enter your Correios Web Services (CWS) credentials
3. Start querying logistics data from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Owners** — quickly estimate shipping costs for customers without leaving the chat.
- **Developers** — verify address data and integrate logistics logic into applications via natural language.
- **Logistics Managers** — track delivery windows and optimize shipping routes across Brazil.


## Available Tools
- **calculate_prices**: Calculate shipping cost for postal services
- **consult_cep**: Consult address information for a ZIP code
- **estimate_delivery_time**: Estimate delivery time between two ZIP codes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Correios do Brazil** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the shipping cost for a 1kg box (20x20x20cm) from 01001000 to 20040002 using SEDEX (04014)."

**🤖 AI Agent:**
> I've calculated the shipping for your SEDEX package. The estimated cost is R$ 32.50 with a delivery window of 1-2 business days.

---

**👤 You:**
> "How long does it take for a PAC delivery from 01310-200 to 70040-900?"

**🤖 AI Agent:**
> The estimated delivery time for PAC (service 04510) between these locations is 8 working days.

---

**👤 You:**
> "What is the address for CEP 01001000?"

**🤖 AI Agent:**
> The CEP 01001-000 corresponds to Praça da Sé, Sé, São Paulo - SP.


## Installation & Usage

To install and use the **Correios do Brazil** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/correios-do-brazil](https://vinkius.com/mcp/correios-do-brazil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
